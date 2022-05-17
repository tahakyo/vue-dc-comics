/* eslint-disable prettier/prettier */
<template>
  <header class="container header">
    <div class="header__logo">
      <img src="../assets/img/dc-logo.png" alt="dc-logo" />
    </div>
    <nav>
      <ul class="header__menu">
        <li><a href="">link title</a></li>
        <li><a href="">link title</a></li>
        <li><a href="">link title</a></li>
        <li><a href="">link title</a></li>
        <li><a href="">link title</a></li>
        <li><a href="">link title</a></li>
        <li><a href="">link title</a></li>
        <li><a href="">link title</a></li>
        <li><a href="">link title</a></li>
        <li><a href="">link title</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
.header {
  display: flex;
  justify-content: space-between;
  min-width: 1000px;
  &__logo {
    width: 5rem;
    padding: 5px;
  }
  nav {
    display: flex;
    align-items: center;
  }
  &__menu {
    display: flex;
    li {
      margin-right: 1rem;
      color: black;
    }
  }
}
</style>
