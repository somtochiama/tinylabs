<template>
  <div class="home">
    <router-link to="/dashboard">Dashboard &rarr;</router-link>
    <router-link to="/login">Login &rarr;</router-link>
  </div>
</template>

<style lang="scss">
  .home {
    a {
      color: #2bda53;
      text-decoration: none;
      padding: 10px;
      margin: 10px;
    }
  }
</style>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "home",
  components: {
    HelloWorld
  }
};
</script>
