<template>
  <nav class="nav">
    <div class="nav__logo">
      <img src="../assets/Bitmap.png" alt="Logo">
    </div>
    <div class="nav__profile">
      <div class="nav__profile-pic">

      </div>
      <div class="nav__profile-text">
        Hi, Joshua
      </div>
      <div class="dropdown">
        <img src="../assets/Icon.png" alt="Logo">
      </div>
    </div>
  </nav>
</template>

<style lang="scss">
  .nav {
    background-color: #fff;
    border: 1px solid rgba(106, 126, 138, 0.1);
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 2rem;
    grid-column: 1 / -1;
    &__profile {
      color: #013C61;
      display: flex;
      align-items: center;

      &-pic {
        height: 30px;
        width: 30px;
        background-color: grey;
        border-radius: 50%;
        display: inline-block;
        margin-right: 1rem;

      }

      &-text {
        margin-right: 1rem;
        font-weight: 500;
      }
    }


  }
</style>