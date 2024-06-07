<template>
  <section id="features" class="features">
    <div class="container">
      <div class="row gy-4 align-items-center features-item">
        <div
          class="col-lg-5 order-2 order-lg-1 text-start"
          data-aos="fade-up"
          data-aos-delay="200"
        >
          <h2>Lorem ipsum dolor</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Nam eum, enim illo totam nihil quasi quia cupiditate eius doloremque exercitationem possimus magnam officiis repellat, nesciunt incidunt ea reprehenderit, dicta blanditiis!
          </p>
        </div>
        <div
          class="col-lg-7 order-1 order-lg-2 d-flex align-items-center"
          data-aos="zoom-out"
          data-aos-delay="100"
        >
          <div class="image-stack">
            <img
              src="https://bootstrapmade.com/demo/templates/Append/assets/img/features-light-1.jpg"
              alt=""
              class="stack-front"
            />
            <img
              src="https://bootstrapmade.com/demo/templates/Append/assets/img/features-light-2.jpg"
              alt=""
              class="stack-back"
            />
          </div>
        </div>
      </div>

    </div>
  </section>
</template>

<style scoped>


    /* Features Section - Home Page
------------------------------*/
.features {
    background-color: white;
    padding: 5rem 0;
}

.features .features-item img {
  box-shadow: 0 15px 30px -10px rgba(0, 0, 0, 0.1);
}


.features .features-item .features-img-bg img {
  position: absolute;
  inset: 0;
  display: block;
  width: 100%;
  height: 100%;
  -o-object-fit: cover;
  object-fit: cover;
}

.features .features-item .image-stack {
  display: grid;
  position: relative;
  grid-template-columns: repeat(12, 1fr);
}

.features .features-item .image-stack .stack-back {
  grid-column: 4/-1;
  grid-row: 1;
  width: 100%;
  z-index: 1;
}

.features .features-item .image-stack .stack-front {
  grid-row: 1;
  grid-column: 1/span 8;
  margin-top: 20%;
  width: 100%;
  z-index: 2;
}
img{
    border-radius: 10px;
}
</style>