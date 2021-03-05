<template>
  <main class="container">
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
    }
  },

  methods: {
    async checkCode(code) {
      if (code.length === 5) {
        try {
          this.guest = await this.$axios.$get(
            'http://23.111.202.11:3000/codes/' + code
          )

          if (!this.guest) {
            this.$refs.start.wrongCode()
          }
        } catch (e) {
          console.log(e)
        }
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
