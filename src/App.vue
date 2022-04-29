<template>
  <div>
    <div class="container header">
      <img src=".\assets\logo.png" alt="#eror" class="logo" />
      <div class="container menu">
        <menu-button :objects="catalogObjects" :name="'Каталог'" />
        <menu-button :objects="aboutObjects" :name="'О нас'" />
        <a href="#" class="menu-element">Блог</a>
        <a href="#" class="menu-element">Контакты</a>
      </div>
    </div>
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
  </div>
</template>

<script>
import menuButton from "./components/menuButton.vue";

export default {
  name: "App",
  components: {
    menuButton,
  },
  data() {
    return {
      activeLanguge: "RUS",
      languages: ["RUS", "ENG", "GER", "FRA"],
      catalogObjects: [
        {
          link: "#",
          name: "object1",
        },
        {
          link: "#",
          name: "object2",
        },
        {
          link: "#",
          name: "object3",
        },
        {
          link: "#",
          name: "object4",
        },
      ],
      aboutObjects: [
        {
          link: "#",
          name: "object",
        },
        {
          link: "#",
          name: "object2",
        },
        {
          link: "#",
          name: "object3",
        },
        {
          link: "#",
          name: "object4",
        },
      ],
    };
  },
  methods: {},
};
</script>

<style src="./css/main.css"></style>
<style src="./css/main-page.css"></style>
