<template>
  <div>
    <my-header :width="width" />
    <div>
      <div class="slaider">
        <div>
          <h2 class="">Lorem ipsum sit amet,</h2>
          <p>
            consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
            labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
            exercitation ullamco laboris nisi ut aliquip ex ea commodo
            consequat. Duis aute irure dolor in reprehenderit in voluptate velit
            esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat
            cupidatat non proident, sunt in culpa qui officia deserunt mollit
            anim id est laborum.
          </p>
          <button>Записаться</button>
        </div>
        <div></div>
      </div>
      <div></div>
    </div>
    <div class="block">
      <h2 class="block-h">Каталог</h2>
      <div class="container grid-1 w-100 center wrap">
        <a href="#" class="catalog-element center">
          <img src="./assets/Rectangle47.png" alt="#eror" class="catalog-img" />
          <p class="catalog-font">Экскурсии-онлайн</p>
        </a>
        <a href="#" class="catalog-element center">
          <img src="./assets/Rectangle47.png" alt="#eror" class="catalog-img" />
          <p class="catalog-font">Экскурсии-онлайн</p>
        </a>
        <a href="#" class="catalog-element center">
          <img src="./assets/Rectangle47.png" alt="#eror" class="catalog-img" />
          <p class="catalog-font">Экскурсии-онлайн</p>
        </a>
      </div>
    </div>
    <div class="block advantages">
      <h2 class="block-h">Почему мы</h2>
      <div class="container wrap center grid-5">
        <my-advantage
          v-for="advantage in advantages"
          :key="advantage.h"
          :h="advantage.h"
          :p="advantage.p"
        />
      </div>
    </div>
    <div class="block events">
      <h2 class="block-h">Популярные мероприятия</h2>
      <div class="container-c">
        div.
      </div>
    </div>
  </div>
</template>

<script>
import myAdvantage from "./components/myAdvantage.vue";
import myHeader from "./components/myHeader.vue";

export default {
  name: "App",
  components: {
    myHeader,
    myAdvantage,
  },
  created() {
    this.width = screen.width;
  },
  data() {
    return {
      width: 0,
      advantages: [
        {
          h: "Первое отличное преимущество",
          p: "consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, ",
        },
        {
          h: "Второе преимущество",
          p: "consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, ",
        },
        {
          h: "Третье преимущество",
          p: "consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, ",
        },
        {
          h: "Четвертое преимущество",
          p: "consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, ",
        },
      ],
    };
  },
  methods: {},
};
</script>

<style src="./css/main.css"></style>
<style src="./css/main-page.css"></style>
