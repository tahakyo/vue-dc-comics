<template>
  <div id="app">
    <!-- header -->
    <header>
      <AppHeader />
    </header>
    <!-- main -->
    <main>
      <ProductList />
    </main>
    <!-- footer -->
    <footer></footer>
  </div>
</template>
<script>
import AppHeader from "./components/AppHeader.vue";
import ProductList from "./components/ProductList.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    ProductList,
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
