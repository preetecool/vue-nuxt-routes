<template>
  <div>
    <input type="text" v-model="userId" />
    <button @click="loadUser">Go to User Page</button>

    <!-- diffrent sections of the nested route will be loaded here with <nuxt-child/>-->
    <nuxt-child />
  </div>
</template>
<script>
import Header from "./../components/TheHeader.vue";
export default {
  layout: "users",

  data() {
    return {
      userId: "",
    };
  },
  methods: {
    loadUser() {
      this.$router.push(`/users/${this.userId}`);
    },
  },
};
</script>
