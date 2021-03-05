<template>
  <main class="container">
    <slot v-if="!guestInfo" name="start" @checkCode="checkSubmit" />
    <slot v-else name="loggedIn" />
  </main>
</template>

<script>
export default {
  name: 'CodeChecker',
  data() {
    return {
      guestInfo: null,
    }
  },
  methods: {
    async checkSubmit(code) {
      console.log(code)
      if (code.length === 5) {
        const result = await this.$axios.$get(
          'http://23.111.202.11:3000/codes/' + code
        )
        console.log(result)
        this.name = result.title
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
