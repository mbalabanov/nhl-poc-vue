<template>
  <div class="container">
    <div class="row mt-2">
      <div class="col-md-8">
        <div
          id="carouselExampleCaptions"
          class="carousel slide"
          data-bs-ride="carousel"
        >
          <div class="carousel-indicators">
            <button
              type="button"
              data-bs-target="#carouselExampleCaptions"
              data-bs-slide-to="0"
              class="active"
              aria-current="true"
              aria-label="Slide 1"
            ></button>
            <button
              type="button"
              data-bs-target="#carouselExampleCaptions"
              data-bs-slide-to="1"
              aria-label="Slide 2"
            ></button>
            <button
              type="button"
              data-bs-target="#carouselExampleCaptions"
              data-bs-slide-to="2"
              aria-label="Slide 3"
            ></button>
          </div>
          <div class="carousel-inner">
            <div class="carousel-item active">
              <img
                src="../assets/images/hockey1.jpg"
                class="d-block w-100 rounded border"
                alt="Carousel Image"
              />
              <div class="carousel-caption d-none d-md-block">
                <h5>First Video Label</h5>
                <p>
                  Some representative placeholder content for the first video.
                </p>
              </div>
            </div>
            <div class="carousel-item">
              <img
                src="../assets/images/hockey2.jpg"
                class="d-block w-100 rounded border"
                alt="Carousel Image"
              />
              <div class="carousel-caption d-none d-md-block">
                <h5>Second Video Label</h5>
                <p>
                  Some representative placeholder content for the second video.
                </p>
              </div>
            </div>
            <div class="carousel-item">
              <img
                src="../assets/images/hockey3.jpg"
                class="d-block w-100 rounded border"
                alt="Carousel Image"
              />
              <div class="carousel-caption d-none d-md-block">
                <h5>Third Video Label</h5>
                <p>
                  Some representative placeholder content for the third video.
                </p>
              </div>
            </div>
          </div>
          <button
            class="carousel-control-prev"
            type="button"
            data-bs-target="#carouselExampleCaptions"
            data-bs-slide="prev"
          >
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
          </button>
          <button
            class="carousel-control-next"
            type="button"
            data-bs-target="#carouselExampleCaptions"
            data-bs-slide="next"
          >
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
          </button>
        </div>
      </div>
      <div class="col-md-4">
        <div height="300px" class="overflow-auto">
          <h3>Explanatory Videos</h3>

          <div class="list-group">
            <a href="#" class="list-group-item list-group-item-action">
              <img src="../assets/images/video.png" width="18"> Cras justo odio
            </a>
            <a href="#" class="list-group-item list-group-item-action"
              ><img src="../assets/images/video.png" width="18"> Dapibus ac facilisis in</a
            >
            <a href="#" class="list-group-item list-group-item-action"
              ><img src="../assets/images/video.png" width="18"> Morbi leo risus</a
            >
            <a href="#" class="list-group-item list-group-item-action"
              ><img src="../assets/images/video.png" width="18"> Porta ac consectetur ac</a
            >
            <a href="#" class="list-group-item list-group-item-action"
              ><img src="../assets/images/video.png" width="18"> Tu quoque, Brute, fili mi</a
            >
            <a href="#" class="list-group-item list-group-item-action"
              ><img src="../assets/images/video.png" width="18"> Idque Caesaris facere voluntate</a
            >
            <a href="#" class="list-group-item list-group-item-action"
              ><img src="../assets/images/video.png" width="18"> Himnes lingua, institutis legibus</a
            >
          </div>
        </div>
      </div>
    </div>
    <div class="row mt-2">
      <div class="col-md-4">
        <div class="card">
          <img
            src="../assets/images/hockey4.jpg"
            class="card-img-top"
            alt="News Image"
          />
          <div class="card-body">
            <h5 class="card-title">Iste tusor nos eludet!</h5>
            <p class="card-text">
              Quo usque tandem abutere, Catilina, patientia nostra? Paullum
              deliquit, ponderibus modulisque suis ratio utitur.
            </p>
            <a href="#" class="btn btn-outline-secondary">Read more</a>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card">
          <img
            src="../assets/images/hockey5.jpg"
            class="card-img-top"
            alt="News Image"
          />
          <div class="card-body">
            <h5 class="card-title">Quam diu etiam furor?</h5>
            <p class="card-text">
              Salutantibus vitae elit libero, a pharetra augue. Contra legem
              facit qui id facit quod lex prohibet. Cum sociis natoque penatibus
              et magnis.
            </p>
            <a href="#" class="btn btn-outline-secondary">Read more</a>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card">
          <img
            src="../assets/images/hockey6.jpg"
            class="card-img-top"
            alt="News Image"
          />
          <div class="card-body">
            <h5 class="card-title">Etiam habebis sem euismod.</h5>
            <p class="card-text">
              Phasellus laoreet lorem vel dolor tempus vehicula. Ullamco laboris
              nisi ut aliquid ex ea commodi consequat.
            </p>
            <a href="#" class="btn btn-outline-secondary">Read more</a>
          </div>
        </div>
      </div>
    </div>
    <div class="row m-4">
      <div class="col text-center">
        <button type="button" class="btn btn-outline-secondary btn-lg">
          More NHL Edge Stories
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Carousel",
  props: {},
};
</script>

<style scoped>
.carousel-caption {
  text-shadow: 0px 0px 2px #000000;
}
</style>
