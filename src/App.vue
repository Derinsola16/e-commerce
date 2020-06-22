<template>
  <div id="app">
    <router-view />
    <AppNav v-if="showMainNav" />
  </div>
</template>

<script>
export default {
  name: "app",
  components: {
    AppNav: () => import("@/components/AppNav.vue")
  },
  computed: {
    showMainNav() {
      return (
        this.$route.name === "home" ||
        this.$route.name == "category" ||
        this.$route.name == "search" ||
        this.$route.name == "profile"
      );
    }
  }
};
</script>

<style>
/* @import "~bootstrap/css/bootstrap"; */
@import "./scss/components/global.scss";
</style>
