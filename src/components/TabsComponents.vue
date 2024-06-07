<template>
  <section id="departments" class="departments py-5">
    <div class="container" data-aos="fade-up">
      <div class="section-title">
        <h2>Lorem ipsum dolor sit.</h2>
        <p>
          Magnam dolores commodi suscipit. Necessitatibus eius consequatur ex
          aliquid fuga eum quidem. Sit sint consectetur velit. Quisquam quos
          quisquam cupiditate. Et nemo qui impedit suscipit alias ea. Quia
          fugiat sit in iste officiis commodi quidem hic quas.
        </p>
      </div>

      <div class="row" data-aos="fade-up" data-aos-delay="100">
        <div class="col-lg-4 mb-5 mb-lg-0">
          <ul class="nav nav-tabs flex-column">
            <li class="nav-item">
              <a
                class="nav-link active show"
                data-bs-toggle="tab"
                data-bs-target="#tab-1"
              >
                <h4>Cardiology</h4>
                <p>
                  Quis excepturi porro totam sint earum quo nulla perspiciatis
                  eius.
                </p>
              </a>
            </li>
            <li class="nav-item mt-2">
              <a class="nav-link" data-bs-toggle="tab" data-bs-target="#tab-2">
                <h4>Neurology</h4>
                <p>Voluptas vel esse repudiandae quo excepturi.</p>
              </a>
            </li>
            <li class="nav-item mt-2">
              <a class="nav-link" data-bs-toggle="tab" data-bs-target="#tab-3">
                <h4>Hepatology</h4>
                <p>Velit veniam ipsa sit nihil blanditiis mollitia natus.</p>
              </a>
            </li>
            <li class="nav-item mt-2">
              <a class="nav-link" data-bs-toggle="tab" data-bs-target="#tab-4">
                <h4>Pediatrics</h4>
                <p>
                  Ratione hic sapiente nostrum doloremque illum nulla
                  praesentium id
                </p>
              </a>
            </li>
          </ul>
        </div>
        <div class="col-lg-8">
          <div class="tab-content">
            <div class="tab-pane active show" id="tab-1">
              <h3>Cardiology</h3>
              <p class="text-start">
                Qui laudantium consequatur laborum sit qui ad sapiente dila
                parde sonata raqer a videna mareta paulona marka
              </p>
              <img
                src="https://bootstrapmade.com/demo/templates/Medicio/assets/img/departments-1.jpg"
                alt=""
                class="img-fluid"
              />
              <p>
                Et nobis maiores eius. Voluptatibus ut enim blanditiis atque
                harum sint. Laborum eos ipsum ipsa odit magni. Incidunt hic ut
                molestiae aut qui. Est repellat minima eveniet eius et quis
                magni nihil. Consequatur dolorem quaerat quos qui similique
                accusamus nostrum rem vero
              </p>
            </div>
            <div class="tab-pane" id="tab-2">
              <h3>Neurology</h3>
              <p class="text-start">
                Qui laudantium consequatur laborum sit qui ad sapiente dila
                parde sonata raqer a videna mareta paulona marka
              </p>
              <img
                src="https://bootstrapmade.com/demo/templates/Medicio/assets/img/departments-1.jpg"
                alt=""
                class="img-fluid"
              />
              <p>
                Et nobis maiores eius. Voluptatibus ut enim blanditiis atque
                harum sint. Laborum eos ipsum ipsa odit magni. Incidunt hic ut
                molestiae aut qui. Est repellat minima eveniet eius et quis
                magni nihil. Consequatur dolorem quaerat quos qui similique
                accusamus nostrum rem vero
              </p>
            </div>
            <div class="tab-pane" id="tab-3">
              <h3>Hepatology</h3>
              <p class="text-start">
                Qui laudantium consequatur laborum sit qui ad sapiente dila
                parde sonata raqer a videna mareta paulona marka
              </p>
              <img
                src="https://bootstrapmade.com/demo/templates/Medicio/assets/img/departments-1.jpg"
                alt=""
                class="img-fluid"
              />
              <p>
                Et nobis maiores eius. Voluptatibus ut enim blanditiis atque
                harum sint. Laborum eos ipsum ipsa odit magni. Incidunt hic ut
                molestiae aut qui. Est repellat minima eveniet eius et quis
                magni nihil. Consequatur dolorem quaerat quos qui similique
                accusamus nostrum rem vero
              </p>
            </div>
            <div class="tab-pane" id="tab-4">
              <h3>Pediatrics</h3>
              <p class="text-start">
                Qui laudantium consequatur laborum sit qui ad sapiente dila
                parde sonata raqer a videna mareta paulona marka
              </p>
              <img
                src="https://bootstrapmade.com/demo/templates/Medicio/assets/img/departments-1.jpg"
                alt=""
                class="img-fluid"
              />
              <p>
                Et nobis maiores eius. Voluptatibus ut enim blanditiis atque
                harum sint. Laborum eos ipsum ipsa odit magni. Incidunt hic ut
                molestiae aut qui. Est repellat minima eveniet eius et quis
                magni nihil. Consequatur dolorem quaerat quos qui similique
                accusamus nostrum rem vero
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
    /*--------------------------------------------------------------
# Departments
--------------------------------------------------------------*/
.departments{
    background-color: white;
}
.departments .nav-tabs {
  border: 0;
}

.departments .nav-link {
  border: 0;
  padding: 20px;
  color: #555555;
  border-radius: 0;
  border-left: 5px solid #fff;
  cursor: pointer;
}

.departments .nav-link h4 {
  font-size: 18px;
  font-weight: 600;
  transition: 0.3s;
}

.departments .nav-link p {
  font-size: 14px;
  margin-bottom: 0;
}

.departments .nav-link:hover h4 {
  color: #3fbbc0;
}

.departments .nav-link.active {
  background: #f7fcfc;
  border-color: #3fbbc0;
}

.departments .nav-link.active h4 {
  color: #3fbbc0;
}

.departments .tab-pane.active {
  animation: slide-down 0.5s ease-out;
}

.departments .tab-pane img {
  float: left;
  max-width: 300px;
  padding: 0 15px 15px 0;
}

@media (max-width: 768px) {
  .departments .tab-pane img {
    float: none;
    padding: 0 0 15px 0;
    max-width: 100%;
  }
}

.departments .tab-pane h3 {
  font-size: 26px;
  font-weight: 600;
  margin-bottom: 20px;
  color: #3fbbc0;
}

.departments .tab-pane p {
  color: #777777;
}

.departments .tab-pane p:last-child {
  margin-bottom: 0;
}

@keyframes slide-down {
  0% {
    opacity: 0;
  }

  100% {
    opacity: 1;
  }
}

</style>