<template>
  <div id="headerCarousel" class="carousel slide" data-bs-ride="carousel">
    <div class="overlay"></div>

    <div class="carousel-inner">
      <div
        class="carousel-item"
        v-for="(slide, key) in carousel"
        :key="key"
        :class="key == 0 ? 'active' : ''"
      >
        <img :src="slide.img" :alt="slide.imgAlt" />
      </div>

      <div
        class="header__content container d-flex justify-content-center align-items-center flex-column"
      >
        <div class="content__text">
          <span>INTERIOR DESIGN COMPANY</span>
          <h1>Experience Interior Design</h1>
        </div>

        <div class="content__cards row">
          <div class="col-4" v-for="(card, key) in cards" :key="key">
            <div
              class="content__card d-flex align-items-center text-start gap-3 p-3"
            >
              <img :src="card.img" :alt="card.imgAlt" />
              <div class="content__card--text">
                <span>{{ card.title }}</span>
                <p>
                  {{ card.text }}
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <button
      class="carousel-control-prev"
      type="button"
      data-bs-target="#headerCarousel"
      data-bs-slide="prev"
    >
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Previous</span>
    </button>
    <button
      class="carousel-control-next"
      type="button"
      data-bs-target="#headerCarousel"
      data-bs-slide="next"
    >
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Next</span>
    </button>
  </div>
</template>

<script setup>
const cards = [
  {
    title: "Interior Architecture",
    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
    img: "https://previews.123rf.com/images/abscent/abscent2002/abscent200200006/139267385-cirug%C3%ADa-personal-en-icono-uniforme-m%C3%A9dico-cirujano-con-mascarilla-asistencia-sanitaria.jpg",
    imgAlt: "image",
  },
  {
    title: "Interior Architecture",
    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
    img: "https://previews.123rf.com/images/abscent/abscent2002/abscent200200006/139267385-cirug%C3%ADa-personal-en-icono-uniforme-m%C3%A9dico-cirujano-con-mascarilla-asistencia-sanitaria.jpg",
    imgAlt: "image",
  },
  {
    title: "Interior Architecture",
    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
    img: "https://previews.123rf.com/images/abscent/abscent2002/abscent200200006/139267385-cirug%C3%ADa-personal-en-icono-uniforme-m%C3%A9dico-cirujano-con-mascarilla-asistencia-sanitaria.jpg",
    imgAlt: "image",
  },
];

const carousel = [
  {
    img: "https://preview.colorlib.com/theme/interiordesign/images/hero_bg_1.jpg.webp",
    imgAlt: "image",
  },
  {
    img: "https://preview.colorlib.com/theme/interiordesign/images/hero_bg_1.jpg.webp",
    imgAlt: "image",
  },
  {
    img: "https://preview.colorlib.com/theme/interiordesign/images/hero_bg_1.jpg.webp",
    imgAlt: "image",
  },
];
</script>

<style scoped>
.carousel-item img {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: auto;
  z-index: -1;
}

#headerCarousel .carousel-item {
  position: relative;
  height: 100vh;
}

.header__content {
  height: 100%;
  position: relative;
  z-index: 1;
  color: white;
  font-family: "Open Sans", sans-serif;

  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.overlay {
  background-color: rgba(0, 0, 0, 0.42);
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  z-index: 1;
}

/* Text */
.content__text {
  text-transform: uppercase;
  width: 55%;
  margin: 0 auto;
}
.content__text h1 {
  font-size: 4.5rem;
}

/* Cards */
.content__cards {
  position: absolute;
  bottom: 0;
  width: 80%;
  margin: 0 auto;

  font-size: 0.9rem;
  padding-bottom: 20px;
}
.content__card {
  background: rgba(0, 0, 0, 0.5);
  color: rgb(161, 161, 161);
  border-radius: 5px;
}

.content__card img {
  width: 60px;
}

.content__card span {
  color: rgb(43, 136, 148);
}
</style>