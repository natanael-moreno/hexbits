<template>
  <section class="bg-white content pt-5">
    <div class="content__top mx-auto">
      <h2>Encuentra con nosotros tu solución</h2>
      <p class="m-0">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Neque
        perferendis atque repellendus a aliquam, nihil in dolor, autem
        praesentium natus officia commodi voluptatum aperiam inventore,
        veritatis unde reiciendis consequatur voluptatem!
      </p>
    </div>

    <div class="pt-4 content__benefits row align-items-center container mx-auto">

      <div class="content__left col-4">
        <div class="content__card d-flex gap-2" v-for="(item, key) in leftItems" :key="key">
          <i class="fa-solid fa-medal"></i>
          <div class="content__card_text text-start">
            <h4>{{ item.title }}</h4>
            <p class="m-0">
              {{ item.text }}
            </p>
          </div>
        </div>
      </div>

      <img class="col-4" :src="require(`../assets/img/medico.png`)" alt=""> 

       <div class="content__right col-4">
        <div class="content__card d-flex gap-2" v-for="(item, key) in rightItems" :key="key">
          <i class="fa-solid fa-medal"></i>
          <div class="content__card_text text-start">
            <h4>{{ item.title }}</h4>
            <p class="m-0">
              {{ item.text }}
            </p>
          </div>
        </div>
      </div>

    </div>
  </section>
</template>

<script setup>
const leftItems = [
  {
    title: "Optimización del Tiempo",
    text: "Registra pacientes, agenda consultas y accede a la información relevante de manera rápida y sencilla, permitiéndote dedicar más tiempo a la atención directa de tus pacientes.",
    icon: "",
  },
  {
    title: "Centralización de la Información",
    text: "Accede a los historiales médicos, odontogramas y registros de consultas desde una única plataforma, eliminando la necesidad de consultar múltiples sistemas o archivos físicos dispersos.",
    icon: "",
  },
];

const rightItems = [
  {
    title: "Mayor Precisión en el Diagnóstico",
    text: "Utiliza el odontograma interactivo para registrar tratamientos, diagnósticos y evolución de cada paciente de forma visual y detallada, lo que te permite llevar un seguimiento más preciso y personalizado de su salud bucal.",
    icon: "",
  },
  {
    title: "Fidelización de Pacientes",
    text: "Ofrece un servicio más completo y personalizado al mantener un historial completo de cada paciente, lo que contribuye a fortalecer la relación médico-paciente y fomentar la fidelidad a tu consulta.",
    icon: "",
  },
];
</script>

<style scoped>
.content__top {
  width: 40%;
}

.content__card {
    margin-top: 4.5rem;
}

.content__card i{
    color: rgb(76, 154, 199);
    padding-top: 7px;
    font-size: 1.5rem;
}
.content__card p{
    font-size: .9rem;
}
</style>