<template>
  <nav class="navbar navbar-expand-lg bg-primary py-5 rounded-4 mt-2 elevation-5">
    <img src="src\assets\img\12791.png" alt="" class="logo elevation-2 rounded-circle" style="width:9%">
    <h2 class="p-2 title text-primary bg-success rounded-pill px-3 fb ">CENTENNIAL HIGH SCHOOL</h2>
    <!-- <router-link class="navbar-brand d-flex" :to="{ name: 'Home' }">
      <div class="d-flex flex-column align-items-center">
        <img alt="logo" src="../assets/img/cw-logo.png" height="45" />
      </div>
    </router-link> -->
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarText"
      aria-controls="navbarText" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div>
      <div class="collapse navbar-collapse mt-5 pt-3" id="navbarText">
        <ul class="navbar-nav me-auto">
          <li>
            <router-link :to="{ name: 'Home' }" class="btn text-light selectable text-uppercase ">
              <h3>HOME</h3>
            </router-link>
          </li>
          <li>
            <router-link :to="{ name: 'About' }" class="btn text-light selectable text-uppercase ">
              <h3>About</h3>
            </router-link>
          </li>

        </ul>
        <!-- LOGIN COMPONENT HERE -->
        <!-- <Login /> -->
      </div>
      <div>
        <div class="bg-success font-primary px-3 my-2 d-flex gap-5 p-2 rounded-3 elevation-5">
          <div class="rounded-2 fw-bold text-primary selectable text-uppercase">Schedule</div>
          <div class="rounded-2 fw-bold text-primary selectable text-uppercase">Coaches</div>
          <div class="rounded-2 fw-bold text-primary selectable text-uppercase">Roster</div>
          <div class="rounded-2 fw-bold text-primary selectable text-uppercase">Summaries & Headlines</div>
          <div class="rounded-2 fw-bold text-primary selectable text-uppercase">News</div>
          <div class="rounded-2 fw-bold text-primary selectable text-uppercase">Photos</div>
          <div class="rounded-2 fw-bold text-primary selectable text-uppercase">Videos</div>
          <div class="rounded-2 fw-bold text-primary selectable text-uppercase">Camps</div>
          <div class="rounded-2 fw-bold text-primary selectable text-uppercase">Team Links</div>
          <div class="rounded-2 fw-bold text-primary selectable text-uppercase">More</div>

        </div>
      </div>
    </div>
  </nav>
</template>

<script>
import Login from './Login.vue'
export default {
  setup() {
    return {}
  },
  components: { Login }
}
</script>

<style scoped>
a:hover {
  text-decoration: none;
}

.nav-link {
  text-transform: uppercase;
}

.navbar-nav .router-link-exact-active {
  border-bottom: 2px solid var(--bs-success);
  border-bottom-left-radius: 0;
  border-bottom-right-radius: 0;
}

.logo {
  position: relative;
  top: 0px;
  left: -18px;
}

.title {
  position: absolute;
  top: -40px;
  left: 120px;
  border-style: solid;
  border-color: rgb(102, 0, 0),
  ;
  border-width: thick;
}


@media screen and (min-width: 768px) {
  nav {
    height: 64px;
  }
}
</style>
