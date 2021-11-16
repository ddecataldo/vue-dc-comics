<template>
  <div class="product-card">

    <img :src="thumb" alt="" />

    <h4>{{ series }}</h4>

  </div>
</template>

<script>
export default {
  name: "ProductCard",
  props: {
    thumb: String,
    price: {
      type: String,
      required: true,
    },
    series: String,
    type: String,
  },
  data() {
    return {};
  },
};
</script>