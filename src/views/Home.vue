<template>
  <div class="home">
    <router-link to="/dashboard">Dashboard</router-link>
    <router-link to="/login">Login</router-link>
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
