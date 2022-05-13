<template>
  <div class="container">
    <div class="row">
      <div class="col-md-3 p-2">
        <img
          src="../assets/nhl-edge.png"
          alt="NHL Edge"
          class="img-fluid"
        />
      </div>
      <div class="col-md-9 p-3">
        <ul class="nav">
          <li class="nav-item">
            <a class="nav-link link-dark active" aria-current="page" href="#"
              >Home</a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link link-dark" href="#">Teams</a>
          </li>
          <li class="nav-item">
            <a class="nav-link link-dark" href="#">Skaters</a>
          </li>
          <li class="nav-item">
            <a class="nav-link link-dark" href="#">Goalies</a>
          </li>
        </ul>
      </div>
    </div>
    <div class="row border-top">
      <div class="col-md-12 px-3 pt-1">
        <nav aria-label="breadcrumb">
          <ol class="breadcrumb">
            <li class="breadcrumb-item"><a href="#">Bread</a></li>
            <li class="breadcrumb-item"><a href="#">Crumb</a></li>
            <li class="breadcrumb-item active" aria-current="page">Current</li>
          </ol>
        </nav>
      </div>
    </div>

    <div class="row">
      <div class="col pt-2 text-center">
        <div class="alert alert-primary" role="alert">
        This is a <strong>proof-of-concept</strong> for Vue3 and chart.js (please scroll down to the players for some charts)
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SubNavigation",
  props: {},
};
</script>

<style scoped>
</style>
