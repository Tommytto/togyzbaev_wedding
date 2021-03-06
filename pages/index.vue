<template>
  <div>
    <code-checker class="desktop" />
    <div class="mobile">
      <div class="hide1-container">
        <h1 class="hide1">СВАДЬБА</h1>
        <div class="hide2">будет 22/08/2021</div>
      </div>
      <div class="hide2-container">
        <img class="hide3" src="~/assets/heart.svg" alt="heart" />
        <div class="hide4">все остальное вы узнаете с десктопной версии</div>
        <div class="hide5">пожалуйста, воспользуйтесь компьютером</div>
      </div>
    </div>
  </div>
</template>

<script>
import CodeChecker from '../components/CodeChecker'
export default {
  components: { CodeChecker },
}
</script>
<style>
.mobile {
  display: none;

  height: 100vh;
  width: 100vw;
  align-items: center;
  font-size: 40px;
  font-weight: bold;
  text-align: center;
  flex-direction: column;
  justify-content: center;
  padding: 30px;
}
@media (max-width: 1200px) {
  .mobile {
    display: flex;
  }

  .desktop {
    display: none !important;
  }
}

.hide1 {
  font-weight: bold;
  font-size: 48px;
  line-height: 58px;
  text-align: center;
  text-transform: uppercase;
}

.hide2 {
  font-style: italic;
  font-weight: 300;
  font-size: 40px;
  line-height: 48px;
  text-align: center;
  margin-top: 24px;
}

.hide2-container {
  margin-top: 101px;
}

.hide4 {
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 19px;
  text-align: center;
  margin-top: 17px;
}

.hide5 {
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 19px;
  text-align: center;
  margin-top: 16px;
}
</style>
