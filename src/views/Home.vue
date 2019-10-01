<template>
  <div class="home">
    <router-link to="/dashboard">Dashboard &rarr; </router-link>
    <router-link to="/login">Login &rarr;</router-link>
  </div>
</template>

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

<style lang="scss">

  .home {
    a {
      text-decoration: none;
      color: #2BDA53;
      display: inline-block;
      padding: 1rem;
      margin: 1rem;
    }
  }
  
</style>
