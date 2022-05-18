<template>
  <section class="product">
    <div class="product__img">
      <img :src="img" alt="" />
    </div>
    <h5>{{ title }}</h5>
  </section>
</template>

<script>
export default {
  name: "AppProduct",
  props: {
    img: String,
    title: String,
  },
};
</script>

<style lang="scss" scoped>
.product {
  width: calc(100% / 6 - 20px);
  margin: 10px;
  &__img {
    height: 150px;
    overflow: hidden;
  }
  h5 {
    padding: 0.5rem 0;
  }
}
</style>
