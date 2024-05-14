<template>
  <div id="app">
    <b-container fluid>
      <Header></Header>
      <Intro></Intro>
      <About></About>
      <Work></Work>
      <Gallery></Gallery>
      <Reviews></Reviews>
      <Order></Order>
      <Footer></Footer>
    </b-container>
  </div>
</template>

<script>
import Header from "./components/header.vue";
import Intro from "./components/intro.vue";
import About from "./components/about.vue";
import Work from "./components/work.vue";
import Gallery from "./components/gallery.vue";
import Reviews from "./components/reviews.vue";
import Order from "./components/order.vue";
import Footer from "./components/footer.vue";

export default {
  name: "App",
  components: {
    Gallery,
    Work,
    About,  
    Header,
    Intro,
    Reviews,
    Order,
    Footer
  },
};
</script>
