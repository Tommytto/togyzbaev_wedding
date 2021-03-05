<template>
  <div class="start">
    <h1 class="start__title">
      <span>Скоро будет</span>
      <span class="thin italic">важное событие!</span>
    </h1>
    <div class="start__help">Введи код, который ты получил</div>
    <div class="start__numbers">
      <input
        ref="number1"
        class="start__number"
        type="text"
        maxlength="1"
        @input="handleChange(1)"
      />
      <input
        ref="number2"
        class="start__number"
        type="text"
        maxlength="1"
        @input="handleChange(2)"
      />
      <input
        ref="number3"
        class="start__number"
        type="text"
        maxlength="1"
        @input="handleChange(3)"
      />
      <input
        ref="number4"
        class="start__number"
        type="text"
        maxlength="1"
        @input="handleChange(4)"
      />
      <input
        ref="number5"
        class="start__number"
        type="text"
        maxlength="1"
        @input="handleChange(5)"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: 'Start',
  methods: {
    getNumber() {
      let value = ''
      for (let i = 0; i < 5; i++) {
        const number = this.$refs['number' + (i + 1)]
        value += number.value
      }

      return value
    },
    handleChange(id) {
      console.log('here')
      this.$emit('checkCode', this.getNumber())
      const next = this.$refs['number' + (id + 1)]
      if (next) {
        next.focus()
      }
    },
  },
}
</script>

<style scoped>
.start {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  flex: 1;
}

.start__title {
  font-weight: bold;
  font-size: 80px;
  line-height: 97px;
}

.start__help {
  font-weight: 500;
  font-size: 32px;
  line-height: 39px;
  margin-top: 80px;
}

.start__numbers {
  display: flex;
  margin-top: 32px;
}

.start__number {
  background: #f5f5f5;
  border-radius: 4px;
  margin-right: 8px;
  border: none;
  width: 80px;
  height: 80px;
  font-size: 40px;
  padding: 28px;
}

.start__number:last-child {
  margin-right: 0;
}
</style>
