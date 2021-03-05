<template>
  <div>
    <code-checker class="desktop" />
    <div class="mobile">СМОТРЕТЬ С КОМПЬЮТЕРА</div>
  </div>
</template>

<script>
import CodeChecker from '../components/CodeChecker'
export default {
  components: { CodeChecker },
}
</script>
<style scoped>
.mobile {
  display: none;

  height: 100vh;
  width: 100vw;
  align-items: center;
  justify-content: center;
  font-size: 40px;
  font-weight: bold;
  text-align: center;
}
@media (max-width: 767px) {
  .mobile {
    display: flex;
  }

  .desktop {
    display: none;
  }
}
</style>
