<template>
  <section class="reviews width-12 grid-12">
    <h2>Отзывы</h2>
    <div class="reviews-gallery width-12 grid-12">
      <div
        class="reviews-gallery-item"
        v-for="review in reviews"
        :key="review.name"
      >
        <img
          class="reviews-gallery-item-icon"
          :src="quoteIcon"
          alt="Quote Icon"
        />
        <span class="reviews-gallery-item-name text-large bold">{{
          review.name
        }}</span>
        <p class="reviews-gallery-item-text">{{ review.text }}</p>
      </div>
    </div>
  </section>
</template>

<script>
import Quote from "../assets/icons/quote.svg";

export default {
  data() {
    return {
      quoteIcon: Quote,
      reviews: [
        {
          name: "Игорь Антонов",
          text: "Обратилась к Aveji по рекомендации. Команда сразу поняла, какой дизайн я хочу. Предоставили несколько вариантов и в течение недели сделали наброски. Итог понравился, все на высшем уровне.",
        },
        {
          name: "Ольга Иванова",
          text: "После пары заказов у компании Aveji убедилась, что за мебелью теперь только к ним. Абсолютно любые решения, в любых размерах и форм-факторе, то что нужно!",
        },
        {
          name: "Аркадий Макаров",
          text: "Aveji — настоящие профессионалы своего дела. Быстро поняли мою задумку, сделали дизайн, согласовали и изготовили мебель. А потом еще и бесплатно все собрали на месте. Большое спасибо!",
        },
      ],
    };
  },
};
</script>
