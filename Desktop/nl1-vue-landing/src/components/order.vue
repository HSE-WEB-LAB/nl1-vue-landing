<template>
  <section class="order-form width-12 grid-12">
    <div class="width-5">
      <img :src="TV" alt="TV">
    </div>
    <div class="width-1"></div>
    <div class="width-6">
      <h2 class="form-title">Хотите заказать проект?</h2>
      <span>Оставьте заявку, и мы вам перезвоним</span>

      <form class="form" action="#" method="POST" @submit.prevent="submitForm">
        <input class="form-text-field" type="text" v-model="name" placeholder="Имя" required>
        <input class="form-text-field" type="text" v-model="email" placeholder="E-mail" required>
        <input class="form-text-field" type="text" v-model="phone" placeholder="Телефон" required>
        <input class="form-text-button" type="submit" value="Отправить заявку">
      </form>

      <div class="mobile-app-links">
        <a href="#"><img :src="appStoreFirst" alt="App Store"></a>
        <a href="#"><img :src="appStoreSecond" alt="Google Play"></a>
      </div>
    </div>
  </section>
</template>

<script>
import TV from "../assets/images/tv.jpg";
import appStoreFirst from "../assets/brands/appstore.png";
import appStoreSecond from "../assets/brands/googleplay.png";

export default {
  data() {
    return {
      name: '',
      email: '',
      phone: ''
    };
  },
  methods: {
    submitForm() {
      // Обработка отправки формы
      console.log('Форма отправлена');
    }
  },
  computed: {
    TV() {
      return TV;
    },
    appStoreFirst() {
      return appStoreFirst;
    },
    appStoreSecond() {
      return appStoreSecond;
    }
  }
};
</script>
