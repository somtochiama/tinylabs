<template>
  <div id="app">
    <div 
        class="btn-app"
        @click="installer()"
        :style="{'display': installBtn}"
        >Add to Home Screen
    </div>
    <button type="button" class="close" aria-label="Close" @click="close">
        <span aria-hidden="true">&times;</span>
    </button>
    <router-view />
  </div>
</template>

<script>
export default {
  data() {
    return {
      installBtn: "none",
      installer: undefined,
      registration: null,
    }
  },
  created() {
    let installPrompt;
    window.addEventListener("beforeinstallprompt", e => {
      e.preventDefault();
      installPrompt = e;
      this.installBtn = "block"
    })
    this.installer = () => {
      this.installBtn = "none";
      installPrompt.prompt();
      installPrompt.userChoice
        .then( result => {
          if(result.outcome === "accepted") {
            console.log("User accepted")
          } else {
            console.log("User denied");
          }
          installPrompt = null
        })
    }
  }
}

</script>

<style lang="scss">
.btn-app {
    background-color: #2BDA53;
    color: white;
    padding: 1rem 4rem;
    border-radius: 3px;
    border: 1px solid #2BDA53;
    display: block
}
</style>
