<template>
  <section>
    <section id="projects" class="projects-section bg-light">
      <div class="container">
        <!-- Featured Project Row -->
        <div
          data-aos="fade-right"
          data-aos-duration="1500"
          class="row align-items-center no-gutters mb-4 mb-lg-5"
        >
          <div class="col-xl-8 col-lg-7">
            <img
              class="img-fluid mb-3 mb-lg-0"
              src="~/assets/punaise_banniere.jpeg"
              alt=""
            />
          </div>
          <div
            data-aos="fade-left"
            data-aos-duration="1500"
            class="col-xl-4 col-lg-5"
          >
            <div class="featured-text text-center text-lg-left">
              <h4>Notre mission</h4>
              <p class="text-black-50 mb-0">
                Pour optimiser la crise gagnant-gagnant, il faut optimiser les
                prestations mobilité.
              </p>
            </div>
          </div>
        </div>

        <!-- Project One Row -->
        <div class="row justify-content-center no-gutters mb-5 mb-lg-0">
          <div data-aos="flip-right" data-aos-duration="1500" class="col-lg-6">
            <img class="img-fluid" src="@/assets/pictos/kesha.svg" alt="" />
          </div>
          <div data-aos="flip-left" data-aos-duration="1500" class="col-lg-6">
            <div class="bg-black text-center h-100 project">
              <div class="d-flex h-100">
                <div
                  class="project-text w-100 my-auto text-center text-lg-left"
                >
                  <h4 class="text-primary-custom">Nettoyages</h4>
                  <p class="mb-0 text-primary-custom-custom">
                    Concomitamment à une dynamique interventionnelle, les
                    sociétés s'engagent à impacter les thématiques dès l'horizon
                    2020.
                  </p>
                  <hr class="d-none d-lg-block mb-0 ml-0" />
                </div>
              </div>
            </div>
          </div>
        </div>

        <!-- Project Two Row -->
        <div class="row justify-content-center no-gutters">
          <div data-aos="flip-right" data-aos-duration="1500" class="col-lg-6">
            <img class="img-fluid" src="@/assets/pictos/spirateur.svg" alt="" />
          </div>
          <div class="col-lg-6 order-lg-first">
            <div class="bg-black text-center h-100 project">
              <div
                data-aos="flip-left"
                data-aos-duration="1500"
                class="d-flex h-100"
              >
                <div
                  class="project-text w-100 my-auto text-center text-lg-right"
                >
                  <h4 class="text-primary-custom">Desinsectisation</h4>
                  <p class="mb-0 text-primary-custom-50">
                    Tangentiellement à la stagflation soutenable, le marché
                    impose d'anticiper les axes mobilisateurs d'excellence.
                  </p>
                  <hr class="d-none d-lg-block mb-0 mr-0" />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Signup Section -->
    <section id="signup" class="signup-section bg-secondary-custom">
      <div class="container">
        <div class="row">
          <div class="col-md-10 col-lg-8 mx-auto text-center">
            <i class="fa fa-paper-plane fa-2x mb-2  text-primary-custom"></i>
            <h2 class="text-primary-custom mb-5">
              Inscrivez vous à la newsletter !
            </h2>

            <form class="form-inline d-flex">
              <input
                id="inputEmail"
                type="email"
                class="form-control flex-fill mr-0 mr-sm-2 mb-3 mb-sm-0"
                placeholder="Entrez votre adresse mail..."
              />
              <button type="submit" class="btn btn-primary mx-auto">
                Valider
              </button>
            </form>
          </div>
        </div>
      </div>
    </section>
  </section>
</template>
