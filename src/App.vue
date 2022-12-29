<template>
  <header class="p-4 mt-3 mb-3">
    <Navbar />
  </header>
  <main>
    <router-view />
  </main>
  <row class="bg-primary" style="height:20px"></row>
  <footer class="text-light bg-dark">
    <div class="d-flex justify-content-center align-items-center bg-dark">

      <div class="col-md-3 d-flex">
        <img src="src\assets\img\12791.png" alt="" class="logo rounded-circle mb-md-2 elevation-3 pb-2 mt-2"
          height="200px" width="200px">
        <div class=" mt-4">
          <p class="info">School Info</p>
          <div>Centennial High School</div>
          <div>12400 West Mc Millan Road</div>
          <div>Boise, ID 83713</div>
          <div>208-855-4250</div>
        </div>
      </div>
      <div class="col-md-6 mt-md-3 ms-md-5 align-content-center">

      </div>
    </div>
  </footer>
</template>
<style>
body.debug .container,
body.debug .container-fluid {
  outline: 2px double blue;
  outline-offset: -2px;
}

body.debug .row {
  outline: 2px dashed red;
  outline-offset: -2px;
}

body.debug [class*="col-"] {
  outline: 2px dotted forestgreen;
  outline-offset: -3px;
}
</style>
<script>
import { computed } from 'vue'
import { AppState } from './AppState'
import Navbar from './components/Navbar.vue'

export default {
  setup() {
    return {
      appState: computed(() => AppState)
    }
  },
  components: { Navbar }
}
</script>
<style lang="scss">
@import "./assets/scss/main.scss";

:root {
  --main-height: calc(100vh - 32px - 64px);
}


// footer {
//   display: grid;
//   place-content: start;
//   height: 180px;
// }

.logo {
  position: relative;
  top: 0px;
  left: 50px;
}

.info {
  font-size: smaller;
  font-weight: bold;
}

@media screen and (min-width: 768px) {
  .logo {
    position: relative;
    top: 0px;
    left: -20px;
  }

}
</style>
