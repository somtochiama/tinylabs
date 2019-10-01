<template>
  <div class="dashboard">
    <TopNav />
    <SideNav />
    <div class="dashboard__body">
      <DashboardHeader />
    </div>
  </div>
</template>

<script>
import TopNav from "../components/TopNav";
import SideNav from "../components/SideNav"
import DashboardHeader from "../components/DashboardHeader"
export default {
  components: {
    TopNav,
    SideNav,
    DashboardHeader
  }
}
</script>

<style lang="scss">
  .dashboard {
    background-color: #f6f8f8;
    height: 100vh;
    display: grid;
    grid-template-rows: 60px auto;
    grid-template-columns: 60px 1fr;
    &__body {
      margin: 6rem 4rem;
    }
  }
</style>