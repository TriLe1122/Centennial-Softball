<template>
  <header class="p-4 mt-3 mb-3">
    <Navbar />
  </header>
  <main class="debug">
    <router-view />
  </main>
  <footer class="bg-dark text-light">
    <div class="row justify-content-center align-items-center g-2">
      <div class="col"><img src="src\assets\img\12791.png" alt="" class="logo rounded-circle" style="width:50%"></div>
      <div class="col">Column</div>
      <div class="col">Column</div>
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


footer {
  display: grid;
  place-content: center;
  height: 32px;
}
</style>
