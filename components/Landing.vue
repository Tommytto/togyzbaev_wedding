<template>
  <div class="landing">
    <div class="landing__date">
      <span class="landing__date-inner">
        <svg
          width="277"
          height="102"
          viewBox="0 0 277 102"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M276.5 51C276.5 57.8436 272.735 64.426 265.788 70.4744C258.841 76.5218 248.761 81.9905 236.262 86.5932C211.266 95.7972 176.702 101.5 138.5 101.5C100.297 101.5 65.7337 95.7972 40.7385 86.5932C28.2389 81.9905 18.1586 76.5218 11.2123 70.4744C4.2649 64.426 0.5 57.8436 0.5 51C0.5 44.1564 4.2649 37.574 11.2123 31.5256C18.1586 25.4782 28.2389 20.0095 40.7385 15.4068C65.7337 6.20275 100.297 0.5 138.5 0.5C176.702 0.5 211.266 6.20275 236.262 15.4068C248.761 20.0095 258.841 25.4782 265.788 31.5256C272.735 37.574 276.5 44.1564 276.5 51Z"
            stroke="black"
          />
        </svg>
        <span class="landing__date-text"> 22/08/2021 </span>
      </span>
    </div>
    <h1 class="landing__title">{{ guest.title }}</h1>
    <div class="landing__invite">
      <span>приглашаем вас на</span><b>WeddingTogShow</b>
    </div>
    <div class="landing__we">
      <img src="~assets/we.png" alt="we" />
    </div>
    <div class="landing__important">
      <div class="landing__part-title"><b>это важно</b> <i>запомнить</i></div>
      <div class="landing__important-place">
        <div class="flex place-1">
          <div>
            <div class="place-title">Когда?</div>
            <div class="place-content">22/08/2021</div>
          </div>
          <div style="margin-left: 127px">
            <div class="place-title">Время?</div>
            <div class="place-content">14:00</div>
          </div>
        </div>
        <div style="margin-top: 48px">
          <div class="place-title">Где?</div>
          <div class="place-content">
            г. Томск, Парк отдыха «Раздолье», с.Богашево, ул.Новостройка,45Н
          </div>
        </div>
      </div>
    </div>
    <div class="landing__star">
      <img class="blue-star" src="~/assets/blue.svg" alt="blue color" />
      <div><b>Под звездочкой</b></div>
      <div style="margin-top: 32px" class="flex">
        <div style="width: 362px">
          До места празднования будет организован трансфер из Томска
        </div>
        <div style="width: 341px; margin-left: 75px">
          После, все иногородние гости остаются ночевать там же
        </div>
      </div>
    </div>
    <div class="landing__color">
      <div class="landing__part-title"><b>Цветовая</b> <i>гамма</i></div>
      <div class="landing__color-container">
        <div class="landing__color-item-container">
          <div class="landing__color-item">
            <img src="~/assets/color-1.svg" alt="color-1" />
          </div>
          <div class="landing__color-title"><b>Сиреневый</b> розовый</div>
        </div>
        <div class="landing__color-item-container">
          <div class="landing__color-item">
            <img src="~/assets/color-2.svg" alt="color-2" />
          </div>
          <div class="landing__color-title"><b>Пряный</b> кофе</div>
        </div>
        <div class="landing__color-item-container">
          <div class="landing__color-item">
            <img src="~/assets/color-3.svg" alt="color-3" />
          </div>
          <div class="landing__color-title"><b>Детский</b> розовый</div>
        </div>
        <div class="landing__color-item-container">
          <div class="landing__color-item">
            <img src="~/assets/color-4.svg" alt="color-4" />
          </div>
          <div class="landing__color-title"><b>Нежный</b> персик</div>
        </div>
        <div class="landing__color-item-container">
          <div class="landing__color-item">
            <img src="~/assets/color-5.svg" alt="color-5" />
          </div>
          <div class="landing__color-title"><b>Вкусный</b> беж</div>
        </div>
      </div>
    </div>
    <div class="landing__color-help">
      <img src="~/assets/heart.svg" alt="heart" />
      <div style="margin-top: 20px">
        <span class="color-help__big">Это означает,</span> что нужно следовать
        именно этой цветовой палитре — никаких синих, желтых, красных и так
        далее! Спасибо!
      </div>
    </div>
    <div class="landing__accent">
      <div class="landing__part-title"><b>яркий</b> <i>акцентный</i></div>
      <div class="landing__accent-info flex">
        <div class="landing__accent-part">
          <div class="flex pink-gold-container">
            <img
              class="pink-gold-img"
              src="~/assets/pink-gold.png"
              alt="ping gold"
            />
            <div class="pink-gold-text"><b>Розовое</b> золото</div>
          </div>
          <div style="margin-bottom: -64px">
            <img class="rose-img" src="~/assets/rose.png" alt="rose" />
          </div>
        </div>
        <div class="landing__accent-part accent-text">
          <div>
            <div style="margin-bottom: 50px">
              цвет,<br />
              который как вишенка на торте
            </div>
            добавь его в свой образ, будет вкусно
          </div>
        </div>
      </div>
    </div>
    <div class="landing__wait">
      <div class="landing__part-title"><b>что</b> <i>вас ждет</i></div>
      <div style="margin-top: 40px; display: flex; flex: 1">
        <div style="flex: 1">
          <div class="wait-text-small">
            <span class="wait-text"> Мы очень любим </span>
            наших гостей
            <br />
            и подготовили незабываемую вечеринку!
          </div>
          <div style="margin-top: 135px; text-align: center">
            <img src="~/assets/we2.png" alt="we" />
          </div>
        </div>
        <div class="wait-text-right" style="flex: 1">
          <div>
            Но мы ничего вам не расскажем, пускай все <br />
            останется в тайне :)
          </div>
          <div style="margin-top: 64px">
            А вот что важно — будет весело, вкусно, <br />
            неожиданно и с любовью!
          </div>
        </div>
      </div>
    </div>
    <div style="margin-top: 188px" class="landing__comment">
      <div class="landing__part-title"><b>давайте</b> <i>по секрету</i></div>
      <div style="margin-top: 48px" class="comment-small">
        <span class="comment-big"> Расскажите, </span>
        есть ли у вас какая-то <br />
        аллергия/особые предпочтения <br />
        в еде? Что-то важное, что мы должны знать о вас?
      </div>
      <form style="margin-top: 56px" @submit.prevent="handleSubmit">
        <textarea
          v-model="comment"
          placeholder="Поле, для ваших мыслей (новый комментарий стирает предыдущий)"
          class="comment-field"
        />
        <div
          style="
            height: 40px;
            margin-top: 8px;
            margin-bottom: -20px;
            font-size: 20px;
          "
        >
          <span v-if="commentSent"> Комментарий отправлен!</span>
        </div>
        <div style="margin-top: 56px">
          <button class="comment-send">Отправить</button>
        </div>
      </form>
    </div>
    <div style="margin-top: 167px" class="landing__come">
      <div class="landing__part-title"><b>нам</b> <i>важно знать</i></div>
      <div style="margin-top: 32px" class="come-help">
        Расскажите, придете вы или нет, пожалуйста!
      </div>
      <div style="width: 830px; margin-top: 48px" class="come-imp">
        <span class="come-imp-big">И очень важно —</span> если вы придете +1 или
        наоборот ваша вторая половинка по каким-то причинам не придет, скажите
        нам сразу, максимально за месяц
      </div>
      <div class="come-button-container" style="max-width: 981px">
        <div
          :class="['come-button', come === 'yes' ? 'active' : '']"
          @click="handleChangeCome('yes')"
        >
          Мы придем
        </div>
        <div
          :class="['come-button', come === 'maybe' ? 'active' : '']"
          @click="handleChangeCome('maybe')"
        >
          Надо подумать
        </div>
        <div
          :class="['come-button', come === 'no' ? 'active' : '']"
          @click="handleChangeCome('no')"
        >
          Спасибо, но нет
        </div>
      </div>
    </div>
    <div style="margin-top: 312px" class="landing__final flex">
      <div>
        <img src="~/assets/we3.svg" alt="we3" />
      </div>
      <div class="final-right" style="margin-left: 50px">
        <div class="landing__part-title"><b>давайте</b> <i>подытожим</i></div>
        <div class="final-place flex" style="margin-top: 74px">
          <div>22 августа 2021</div>
          <div style="margin-left: 85px">в 14:00</div>
        </div>
        <div class="final-place" style="margin-top: 44px">
          г. Томск, Парк отдыха «Раздолье», с.Богашево, ул.Новостройка,45Н
        </div>
        <div class="final-final" style="margin-top: 148px">
          Спасибо за внимание и до встречи, друзья!
        </div>
        <div class="final-final" style="margin-top: 20px; margin-bottom: 100px">
          Не передавайте эту ссылку третьим лицам, это только для вас!
        </div>
      </div>
    </div>
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
  data() {
    return {
      comment: '',
      come: this.guest.come || 'maybe',
      commentSent: false,
    }
  },
  methods: {
    async handleSubmit() {
      this.commentSent = false
      await this.$axios.post(
        `https://api.togyzbaev.com/comments/${this.guest.code}`,
        {
          comment: this.comment,
        }
      )
      this.commentSent = true
    },
    handleChangeCome(come) {
      this.come = come
      this.$axios.post(`https://api.togyzbaev.com/come/${this.guest.code}`, {
        come,
      })
    },
  },
}
</script>

<style scoped>
.landing__final {
  align-items: flex-end;
}
.flex {
  display: flex;
}
.landing {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  flex: 1;
  padding-left: 80px;
  padding-right: 80px;
  max-width: 1440px;
  margin: auto;
}

.landing__date {
  display: flex;
  justify-content: center;
  margin-top: 83px;
}
.landing__date-inner {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
}
.landing__date-text {
  position: absolute;
  font-weight: bold;
  font-size: 36px;
  line-height: 44px;
}
.landing__title {
  font-weight: bold;
  font-size: 128px;
  line-height: 155px;
  text-transform: uppercase;
  margin-top: 62px;
}

.landing__invite {
  font-size: 36px;
  line-height: 44px;
  font-weight: 300;
}

.landing__we {
  margin-top: 127px;
}

.landing__part-title {
  font-weight: 300;
  font-size: 64px;
  line-height: 164%;
  text-transform: uppercase;
}
.landing__important {
  width: 100%;
  text-align: left;
  margin-top: 162px;
}
.landing__important-place {
  margin-top: 100px;
  justify-content: center;
  margin-left: 25vw;
}
.landing__color {
  margin-top: 248px;
}
.place-title {
  font-weight: 300;
  font-size: 20px;
  line-height: 24px;
}

.place-content {
  font-weight: bold;
  font-size: 40px;
  line-height: 48px;
}

.landing__star {
  margin-top: 160px;
  font-weight: normal;
  font-size: 28px;
  line-height: 34px;
  width: 100%;
  justify-content: flex-start;
  text-align: left;
  position: relative;
}
.blue-star {
  position: absolute;
  left: -100px;
  top: -100px;
  z-index: -1;
}
.landing__color {
  width: 100%;
  text-align: left;
  justify-content: flex-start;
}

.landing__color-container {
  display: flex;
  margin-top: 80px;
  flex-wrap: wrap;
}
.landing__color-item {
  display: flex;
}
.landing__color-title {
  margin-top: 47px;
  font-weight: 300;
  font-size: 20px;
  line-height: 24px;
  white-space: nowrap;
}

.landing__color-item-container {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  margin-right: 90px;
}

.landing__color-help {
  margin-top: 238px;
  font-weight: normal;
  font-size: 20px;
  line-height: 32px;
  width: 385px;
}

.color-help__big {
  font-weight: 500;
  font-size: 36px;
  line-height: 158.1%;
}

.landing__accent {
  width: 100%;
  text-align: left;
  justify-content: left;
  margin-top: 211px;
}
.landing__accent-part {
  flex: 1;
  display: flex;
}
.pink-gold-img {
  border-radius: 16px;
  width: 190px;
}
.pink-gold-text {
  font-weight: 300;
  font-size: 28px;
  line-height: 34px;
  transform: rotate(-90deg);
  margin-left: -60px;
  margin-bottom: 71px;
}
.pink-gold-container {
  display: flex;
  justify-content: flex-start;
  align-items: flex-end;
}
.rose-img {
  width: 190px;
  height: 600px;
  object-fit: cover;
}
.accent-text {
  align-items: center;
  font-weight: normal;
  font-size: 24px;
  line-height: 132.5%;
}
.landing__wait {
  margin-top: 256px;
  width: 100%;
  text-align: left;
  justify-content: flex-start;
}
.wait-text {
  font-weight: normal;
  font-size: 36px;
  line-height: 57px;
}

.wait-text-small {
  font-size: 24px;
  line-height: 38px;
}
.wait-text-right {
  font-weight: 300;
  font-size: 24px;
  line-height: 158.1%;
  margin-top: 14px;
}

.comment-big {
  font-weight: 500;
  font-size: 36px;
  line-height: 158.1%;
}
.comment-small {
  font-weight: 300;
  font-size: 24px;
  line-height: 38px;
}
.comment-field {
  background: rgba(232, 224, 218, 0.19);
  border: 1px solid #e8e0da;
  border-radius: 8px;
  height: 198px;
  width: 580px;
  padding: 24px;
  font-weight: normal;
  font-size: 16px;
  line-height: 158.1%;
}
.comment-send {
  background: #e8e0da;
  padding: 24px 54px;
  font-weight: bold;
  font-size: 18px;
  line-height: 158.1%;
  border-radius: 50%;
  outline: none;
  cursor: pointer;
}

.comment-send:active,
.comment-send:hover,
.comment-send:focus {
  background: #fbf9f8;
  border: 1px solid #e8e0da;
}

.come-help {
  font-style: italic;
  font-weight: normal;
  font-size: 24px;
  line-height: 158.1%;
}
.come-imp {
  font-style: normal;
  font-weight: 300;
  font-size: 24px;
  line-height: 38px;
}

.come-imp-big {
  font-style: normal;
  font-weight: 500;
  font-size: 36px;
  line-height: 158.1%;
}
.come-button-container {
  display: flex;
  justify-content: space-between;
  margin-top: 166px;
}

.come-button {
  font-style: normal;
  font-weight: 300;
  font-size: 40px;
  line-height: 48px;
  position: relative;
  padding-bottom: 2px;
  cursor: pointer;
  border-bottom: 1px solid transparent;
}

.come-button:hover,
.come-button:active {
  border-bottom: 1px solid black;
}
.come-button.active {
  font-weight: bold;
}
.come-button.active::before {
  content: url('~/assets/heart.svg');
  position: absolute;
  left: -37px;
  top: 3px;
}

.final-place {
  font-style: normal;
  font-weight: bold;
  font-size: 32px;
  line-height: 39px;
}

.final-final {
  font-style: italic;
  font-weight: normal;
  font-size: 24px;
  line-height: 158.1%;
}
.final-right {
  text-align: left;
}
</style>
