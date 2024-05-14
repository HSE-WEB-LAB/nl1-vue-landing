<template>
  <section class="about width-12 grid-12">
    <div class="width-6">
      <h2>Более 5 лет создаем<br />мебель для вашего<br />комфорта</h2>
    </div>
    <div class="width-6 about-text">
      <p>
        Мы — команда профессионалов, которые могут произвести любую мебель
        для<br />вашего проекта, а также найти производственное<br />решение
        любой задумки.
      </p>
      <p>
        Наша основная цель — реализовывать самые смелые задумки, и делать это
        качественно и аккуратно.
      </p>
      <p>
        В качестве материалов мы используем натуральные — стекло, дерево, бетон,
        камень, металл и эпоксидную смолу.
      </p>
      <div class="about-text-points">
        <div class="about-text-point">
          <h3 class="about-text-point-heading">1 год</h3>
          <span class="about-text-point-desc">гарантия на всю продукцию</span>
        </div>
        <div class="about-text-point">
          <h3 class="about-text-point-heading">300+</h3>
          <span class="about-text-point-desc">выполненных проектов</span>
        </div>
        <div class="about-text-point">
          <h3 class="about-text-point-heading">15 дней</h3>
          <span class="about-text-point-desc">срок производства</span>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "features",
  data() {
    return {
      catalog: [
        {
          number: "30",
          number_descr: "позиций",
          number_descr_2: "Более",
          descr:
            "Мы изготавливаем более 30 видов деревянных накладок, и продолжаем разрабатывать новые дизайны и функциональность изделий!",
          img: [
            { src: "./images/feature/type_1_pad.jpg", alt: "накладка_1_типа" },
            { src: "./images/feature/type_2_pad.jpg", alt: "накладка_2_типа" },
          ],
        },
        {
          number: "8",
          number_descr: " Диаметров бревна",
          number_descr_2: "",
          descr:
            "Мы разработали изделия для 8 самых распространенных размеров бревен. Если у Вас нестандартное бревно, то пишите - мы обязательно что-нибудь придумаем!",
          img: [
            { src: "./images/feature/diameters.png", alt: "диаметр_бревна" },
          ],
        },
        {
          number: "3",
          number_descr: " Вида материала",
          number_descr_2: "",
          descr:
            " Компания создает изделия любого оттенка дерева из трех плотных материалов: сосна, ясень, бук, дуб.",
          img: [
            { src: "./images/feature/pine.jpg", alt: "сосна" },
            { src: "./images/feature/ash.jpg", alt: "Ясень" },
            { src: "./images/feature/beech.jpg", alt: "бук" },
            { src: "./images/feature/oak.jpg", alt: "дуб" },
          ],
        },
        {
          number: "2",
          number_descr: "Типа стен",
          number_descr_2: "",
          descr:
            "Наши изделия предусмотрены для бревенчатых стен и блок-хауса.",
          img: [
            { src: "./images/feature/log.jpg", alt: "бревенчатые" },
            { src: "./images/feature/block-house.jpg", alt: "блок-хаус" },
          ],
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss"></style>
