<template>
  <div class="start">
    <h1 class="start__title">
      <span>Скоро будет</span>
      <span class="thin italic">важное событие!</span>
    </h1>
    <div class="start__help">Введи код, который ты получил</div>
    <div class="start__numbers">
      <input
        v-for="number in fields"
        :key="number"
        :ref="'number' + number"
        class="start__number"
        type="text"
        maxlength="1"
        @input="handleChange(number)"
      />
    </div>
    <div class="start__error">
      <span v-if="error"> Неправильный код, попробуйте еще раз </span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Start',
  data() {
    return {
      error: false,
      fields: [1, 2, 3, 4, 5],
    }
  },
  methods: {
    getNumber() {
      return this.fields.map((num) => this.getField(num).value).join('')
    },
    handleChange(id) {
      this.error = false
      this.$emit('checkCode', this.getNumber())
      const current = this.getField(id)
      const next = this.getField(id + 1)
      if (next && current && current.value) {
        next.focus()
        next.select()
      }
    },
    getField(num) {
      return this.$refs['number' + num] && this.$refs['number' + num][0]
    },
    wrongCode() {
      this.error = true
      this.fields.forEach((number) => {
        const numberField = this.getField(number)
        numberField.value = ''
      })
      this.getField(this.fields[0]).focus()
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
  width: 80px;
  height: 80px;
  font-size: 40px;
  padding: 28px;
}

.start__number:hover,
.start__number:active,
.start__number:focus {
  border: 1px solid #c7c7c7;
}

.start__number:last-child {
  margin-right: 0;
}

.start__error {
  color: red;
  height: 15px;
  font-size: 20px;
  margin-top: 8px;
}
</style>
