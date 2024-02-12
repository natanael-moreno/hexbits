<template>
  <section class="p-5" style="background-color: #edf2f9">
    <div class="container pt-5">
      <div class="row justify-content-center text-center">
        <div class="col-lg-8 col-xl-7 col-xxl-6">
          <h1 class="fs-2 fs-sm-4 fs-md-5">WebApp theme of the future</h1>
          <p class="lead">
            Built on top of Bootstrap 5, super modular Falcon provides you
            gorgeous design &amp; streamlined UX for your WebApp.
          </p>
        </div>
      </div>

      <div
        class="row justify-content-center align-items-center mt-5"
        v-for="(item, key) in items"
        :key="key"
        :class="key % 2 == 0 ? 'text-start' : 'text-end'"
      >
        <div
          class="col-md col-lg-5 col-xl-4 ps-lg-6"
          :class="key % 2 != 0 ? 'order-md-2' : ''"
        >
          <img
            class="img-fluid px-6 px-md-0"
            :src="require(`../assets/img/${item.img}`)"
            :alt="item.imgAlt"
          />
        </div>
        <div class="col-md col-lg-5 col-xl-4 mt-4 mt-md-0">
          <h5
            class="text-info"
            :class="key > 0 && key == 1 ? 'text-danger' : ''"
          >
            <span class="fas fa-pump-medical me-2"></span>{{ item.subtitle }}
          </h5>
          <h3>{{ item.title }}</h3>
          <p>
            {{ item.text }}
          </p>
        </div>
      </div>
    </div>
    <!-- end of .container-->
  </section>
</template>

<script setup>
const items = [
  {
    title: "Titulo 1",
    subtitle: "Subtitulo 1",
    text: "Texto de prueba",
    img: "doctor.png",
    imgAlt: "Imagen",
  },
  {
    title: "Titulo 2",
    subtitle: "Subtitulo 2",
    text: "Texto de prueba",
    img: "doctor.png",
    imgAlt: "Imagen",
  },
  {
    title: "Titulo 3",
    subtitle: "Subtitulo 3",
    text: "Texto de prueba",
    img: "doctor.png",
    imgAlt: "Imagen",
  },
];
</script>