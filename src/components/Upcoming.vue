<template>
  <h3 class="p-2 fw-bold text-secondary">Upcoming Games</h3>
  <div class="border">

    <div class="card border-0 border-bottom">
      <div class="card-body">
        <h6 class="card-title fw-bold text-secondary"> <i class="mdi mdi-bus text-danger fs-5"></i> Thursday Mar 9 @ 5:00PM (A)</h6>
        <p class="fontsize">vs <a href="url">Mountain View High School</a></p>
      </div>
    </div>
    <div class="card border-0 border-bottom">
      <div class="card-body">
        <h6 class="card-title fw-bold text-secondary"> <i class="mdi mdi-bus text-danger fs-5"></i> Friday Mar 10 @ 5:00PM (A)</h6>
        <p class="fontsize">vs <a href="url">Caldwell High School</a></p>
      </div>
    </div>
    <div class="card border-0">
      <div class="card-body">
        <h6 class="card-title fw-bold text-secondary"> <i class="mdi mdi-bus text-danger fs-5"></i> Saturday Mar 11 @ 5:00PM (A)</h6>
        <p class="fontsize">vs <a href="url">Meridian High School</a></p>
      </div>
    </div>

  </div>
</template>


<script>
export default {
  setup() {
    return {}
  }
}
</script>


<style lang="scss" scoped>
.fontsize {
  font-size: .9em;
}
</style>