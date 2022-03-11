<template>
  <div>
    <Header />
    <header>User Header from ./layouts/users.vue</header>
    <Nuxt />
  </div>
</template>
<script>
import Header from "../components/TheHeader.vue";
export default {
  components: {
    Header,
  },
};
</script>
