<template>
  <header class="header width-12 grid-12">
    <div class="width-8">
      <img :src="icon" alt="Icon" />
    </div>
    <div class="navigation-contacts width-4">
      <nav class="navigation">
        <ul>
          <li><a class="text-large" href="#about">О нас</a></li>
          <li><a class="text-large" href="#projects">Проекты</a></li>
          <li><a class="text-large" href="#how-we-work">Материалы</a></li>
          <li><a class="text-large" href="#reviews">Отзывы</a></li>
        </ul>
      </nav>
      <span class="text-large">+7 999 999 99 99</span>
    </div>
  </header>
</template>

<script>
import Icon from "../assets/images/logo.svg";

export default {
  name: "navbar",
  data() {
    return {
      isExpanded: false,
      icon: Icon,
    };
  },
  methods: {
    scrollToTop() {
      window.scrollTo({ top: 0, left: 0, behavior: "smooth" });
    },
    scrollToId(event) {
      let offsetY = 20;
      if (this.isExpanded) {
        let nav = document.getElementById("Nav");
        let bounds = nav.getBoundingClientRect();
        offsetY = bounds.height;
      }
      let element = document.getElementById(event.target.hash.replace("#", ""));
      window.scrollTo({
        top: element.offsetTop - offsetY,
        left: 0,
        behavior: "smooth",
      });
      event.preventDefault();
    },
  },
};
</script>
