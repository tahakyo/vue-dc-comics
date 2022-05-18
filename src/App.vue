<template>
  <div id="app">
    <!-- header -->
    <header>
      <AppHeader />
    </header>
    <!-- main -->
    <main>
      <AppBanner />
      <ProductList />
    </main>
    <!-- footer -->
    <footer></footer>
  </div>
</template>
<script>
import AppHeader from "./components/AppHeader.vue";
import ProductList from "./components/ProductList.vue";
import AppBanner from "./components/AppBanner.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    ProductList,
    AppBanner,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
main {
  background-color: black;
  color: white;
}
</style>
