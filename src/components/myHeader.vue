<template>
  <div class="container header">
    <img src=".\assets\logo.png" alt="#eror" class="logo" />
    <div class="container menu">
      <menu-button :objects="catalogObjects" :name="'Каталог'" />
      <menu-button :objects="aboutObjects" :name="'О нас'" />
      <a href="#" class="menu-element">Блог</a>
      <a href="#" class="menu-element">Контакты</a>
      <button class="menu-button">
        <button-lang :name="activeLanguge" />
      </button>
    </div>
  </div>
</template>

<script>
import menuButton from "./menuButton.vue";
import buttonLang from "./buttonLang.vue";

export default {
  components: {
    menuButton,
    buttonLang,
  },

  data() {
    return {
      languages: ["RUS", "ENG", "GER", "FRA"],
      activeLanguge: "ENG",
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

  props: {
    width: {
      type: Number,
      required: false,
    },
  },
};
</script>

<style src="./css/my-header.css"></style>
