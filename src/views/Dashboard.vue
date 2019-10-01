<template>
  <div class="dashboard">
    <TopNav />
    <SideNav />
    <div class="dashboard__body">
      <DashboardHeader />
      <DashboardTable />
    </div>
  </div>
</template>

<script>
import TopNav from "../components/TopNav";
import SideNav from "../components/SideNav"
import DashboardHeader from "../components/DashboardHeader"
import DashboardTable from "../components/DashboardTable"
export default {
  components: {
    TopNav,
    SideNav,
    DashboardHeader,
    DashboardTable
  }
}
</script>

<style lang="scss">
  .dashboard {
    background-color: #f6f8f8;
    // height: 100vh;
    display: grid;
    grid-template-rows: 60px auto;
    grid-template-columns: 60px 1fr;
    color: #6A7E8A;
    &__body {
      margin: 6rem 4rem;
    }

    &__header {
      
      &-top {
        display: flex;
        justify-content: space-between;
        align-items: center;
      }

      &-info {
        display: flex;
        justify-content: space-between;
        align-items: center;
        background-color: white;
        margin: 2rem 0;
        padding: 3rem 2.5rem;
        border-radius: 5px;
      }
    }
  }
</style>