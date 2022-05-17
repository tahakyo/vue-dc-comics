/* eslint-disable prettier/prettier */
<template>
  <header class="container header">
    <div class="header__logo">
      <img src="../assets/img/dc-logo.png" alt="dc-logo" />
    </div>
    <nav>
      <ul class="header__menu">
        <li
          v-for="(item, index) in MenuLinks"
          :key="index"
          :class="{ active: item.active }"
        >
          <a href="">{{ item.text }}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  data: function () {
    return {
      MenuLinks: [
        {
          url: "#",
          text: "Characters",
          active: false,
        },
        {
          url: "#",
          text: "Comics",
          active: true,
        },
        {
          url: "#",
          text: "Movies",
          active: false,
        },
        {
          url: "#",
          text: "TV",
          active: false,
        },
        {
          url: "#",
          text: "Games",
          active: false,
        },
        {
          url: "#",
          text: "Collectibles",
          active: false,
        },
        {
          url: "#",
          text: "Videos",
          active: false,
        },
        {
          url: "#",
          text: "Fans",
          active: false,
        },
        {
          url: "#",
          text: "News",
          active: false,
        },
        {
          url: "#",
          text: "Shop",
          active: false,
        },
      ],
    };
  },
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
      color: $brand-secondary-color;
      &.active {
        border-bottom: 3px solid $brand-primary-color;
      }
    }
  }
}
</style>
