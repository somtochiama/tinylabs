<template>
  <div class="dashboard__header">
    <div class="dashboard__header-top">
      <h2 class="heading--primary">Employees</h2>
      <MyBtn>Add New</MyBtn>
    </div>
    <div class="dashboard__header-info">
      <h3 class="heading--secondary">Josh Bakery Ventures</h3>
      <p class="dashboard__header-address">62, Bode Thomas, Surukere, Lagos</p>
    </div>
  </div>
</template>

<script>
import MyBtn from "../components/Button"
export default {
  components: {
    MyBtn
  }
}
</script>

<style lang="">
  
</style>