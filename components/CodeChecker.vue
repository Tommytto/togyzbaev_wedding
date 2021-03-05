<template>
  <main v-if="checked" class="container">
    <start v-if="!guest" ref="start" @checkCode="checkCode" />
    <landing v-else :guest="guest" />
  </main>
</template>

<script>
import Start from './Start'
import Landing from './Landing'
export default {
  name: 'CodeChecker',
  components: { Landing, Start },
  data() {
    return {
      guest: null,
      checked: false,
    }
  },
  mounted() {
    this.checkCodeLocal()
  },
  methods: {
    async checkCode(code) {
      if (code.length === 5) {
        try {
          this.guest = await this.getGuest(code)

          if (!this.guest) {
            this.$refs.start.wrongCode()
          } else {
            this.saveCode(code)
          }
        } catch (e) {
          console.log(e)
        }
      }
    },
    getGuest(code) {
      return this.$axios.$get('http://23.111.202.11:3000/codes/' + code)
    },
    saveCode(code) {
      localStorage.setItem('code', code)
    },
    removeCode() {
      localStorage.removeItem('code')
    },
    async checkCodeLocal() {
      const code = localStorage.getItem('code')
      try {
        if (code) {
          const result = await this.getGuest(code)
          if (!result) {
            this.removeCode()
          } else {
            this.guest = result
          }
        }
      } catch (e) {
        this.removeCode()
      } finally {
        this.checked = true
      }
    },
  },
}
</script>
<style scoped>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
}
</style>
