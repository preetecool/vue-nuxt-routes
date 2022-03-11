<template>
  <div>
    <!-- a tag does not prevent the default of sending a request. -->
    <!-- <a href="/users">Users</a> -->
    <!-- router link / nuxt link does prevent it. -->
    <nuxt-link to="/users">Users</nuxt-link>
    <button @click="goToProducts">Products</button>
  </div>
</template>

<script>
export default {
  name: "IndexPage",

  methods: {
    goToProducts() {
      this.$router.push("/products");
    },
  },
};
</script>
