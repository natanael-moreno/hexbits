<template>
  <section style="position: relative; display: flex; justify-content: center; align-items: center; height: 40vh;">
    <!-- Imagen de fondo -->
    <div
      class="background-image"
      :style="{
        backgroundImage: `url(${require('../assets/img/overlay.jpg')})`,
        backgroundPosition: 'center',
      }"
    ></div>

    <!-- Contenido -->
    <div class="container">
      <div class="row justify-content-center text-center">
        <div class="col-lg-8">
          <p class="fs-3 fs-sm-4 text-white">
            Join our community of 20,000+ developers and content creators on
            their mission to build better sites and apps.
          </p>
          <button
            class="btn btn-outline-light border-2 rounded-pill btn-lg mt-4 fs-0 py-2"
            type="button"
          >
            Start your webapp
          </button>
        </div>
      </div>
    </div>
  </section>
</template>

<style>
.background-image {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  filter: brightness(0.5); /* Reduce el brillo de la imagen */
  z-index: -1; /* Coloca la capa detrás del contenido */
}
</style>
