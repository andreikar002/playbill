<template>
  <div
    class="menu-button container center w-100"
    :style="{
      backgroundImage: '(./assets/' + name + 'pick.png)',
    }"
  >
    <p class="pLang">{{ name }}</p>
    <img v-if="isActive" src="./assets/to_down.png" alt="" />
    <img v-else src="./assets/to_up.png" alt="" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      isActive: false,
    };
  },

  props: {
    name: {
      type: String,
      required: false,
    },
  },

  methods: {
    consoleMenuChange() {
      this.isActive = !this.isActive;
    },
  },
};
</script>
