<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark p-4">
    <div class="container-fluid">
      <a class="navbar-brand" href="#"
        ><img
          src="../assets/nhl.svg"
          alt="NHL"
          class="img-fluid"
          height="100"
          width="50"
      /></a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">Scores</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">News</a>
          </li>
          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              href="#"
              id="navbarDropdown"
              role="button"
              data-bs-toggle="dropdown"
              aria-expanded="false"
            >
              Links
            </a>
            <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
              <li><a class="dropdown-item" href="#">Action</a></li>
              <li><a class="dropdown-item" href="#">Another action</a></li>
              <li><hr class="dropdown-divider" /></li>
              <li>
                <a class="dropdown-item" href="#">Something else here</a>
              </li>
            </ul>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">Videos</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">Standings</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">Stats</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">Schedule</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">Players</a>
          </li>
        </ul>
        <form class="d-flex">
          <input
            class="form-control me-2"
            type="search"
            placeholder="Search"
            aria-label="Search"
          />
          <button class="btn btn-outline-light" type="submit">Search</button>
        </form>
      </div>
    </div>
  </nav>
</template>

<script>
  export default {
    name: "MainNavigation",
    props: {
    },
  }
</script>

<style scoped>

</style>
