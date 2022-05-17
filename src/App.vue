<template>
  <div id="app">
    <!-- header -->
    <header>
      <AppHeader />
    </header>
    <!-- main -->
    <main class="container">questo è main</main>
    <!-- footer -->
    <footer></footer>
  </div>
</template>
<script>
import AppHeader from "./components/AppHeader.vue";

export default {
  name: "App",
  components: {
    AppHeader,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
main {
  height: 150px;
  background-color: black;
  color: white;
}
</style>
