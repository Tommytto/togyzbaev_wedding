<template>
  <div class="landing">
    <h1 class="start__title">Ждем вас {{ guest.title }}</h1>
  </div>
</template>

<script>
export default {
  name: 'Landing',
  props: {
    guest: {
      type: Object,
      default: () => ({}),
    },
  },
}
</script>

<style scoped>
.landing {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  flex: 1;
}
</style>
