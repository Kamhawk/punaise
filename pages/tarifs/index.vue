<template>
  <section class="pricing py-5">
    <div class="container">
      <div class="row">
        <!-- Free Tier -->
        <div class="col-lg-4">
          <div class="card mb-5 mb-lg-0">
            <div class="card-body">
              <h5 class="card-title text-muted text-uppercase text-center">
                Nettoyage
              </h5>
              <h6 class="card-price text-center">
                €250<span class="period">/intervention</span>
              </h6>
              <hr />
              <ul class="fa-ul">
                <li>
                  <span class="fa-li"><i class="fa fa-check"></i></span>Un
                  intervenant
                </li>
                <li>
                  <span class="fa-li"><i class="fa fa-check"></i></span>En
                  Semaine
                </li>
                <li>
                  <span class="fa-li"><i class="fa fa-check"></i></span>Produits
                  écologiques
                </li>
                <li>
                  <span class="fa-li"><i class="fa fa-check"></i></span>...
                </li>
                <li class="text-muted">
                  <span class="fa-li"><i class="fa fa-times"></i></span>....
                </li>
                <li class="text-muted">
                  <span class="fa-li"><i class="fa fa-times"></i></span>...
                </li>
                <li class="text-muted">
                  <span class="fa-li"><i class="fa fa-times"></i></span>...
                </li>
                <li class="text-muted">
                  <span class="fa-li"><i class="fa fa-times"></i></span>...
                </li>
              </ul>
              <a href="#" class="btn btn-block btn-primary text-uppercase"
                >Commander</a
              >
            </div>
          </div>
        </div>
        <!-- Plus Tier -->
        <div class="col-lg-4">
          <div class="card mb-5 mb-lg-0">
            <div class="card-body">
              <h5 class="card-title text-muted text-uppercase text-center">
                Désinsectification
              </h5>
              <h6 class="card-price text-center">
                €650<span class="period">/intervention</span>
              </h6>
              <hr />
              <ul class="fa-ul">
                <li>
                  <span class="fa-li"><i class="fa fa-check"></i></span
                  ><strong>Equipe du jour</strong>
                </li>
                <li>
                  <span class="fa-li"><i class="fa fa-check"></i></span>Produits
                  écologique
                </li>
                <li>
                  <span class="fa-li"><i class="fa fa-check"></i></span
                  >Efficacité garantie
                </li>
                <li>
                  <span class="fa-li"><i class="fa fa-check"></i></span>...
                </li>
                <li>
                  <span class="fa-li"><i class="fa fa-check"></i></span>...
                </li>
                <li>
                  <span class="fa-li"><i class="fa fa-check"></i></span>...
                </li>
                <li>
                  <span class="fa-li"><i class="fa fa-check"></i></span>...
                </li>
                <li class="text-muted">
                  <span class="fa-li"><i class="fa fa-times"></i></span>...
                </li>
              </ul>
              <a href="#" class="btn btn-block btn-primary text-uppercase"
                >COmmander</a
              >
            </div>
          </div>
        </div>
        <!-- Pro Complet -->
        <div class="col-lg-4">
          <div class="card">
            <div class="card-body">
              <h5 class="card-title text-muted text-uppercase text-center">
                Pro
              </h5>
              <h6 class="card-price text-center">
                Sur devis
              </h6>
              <hr />
              <ul class="fa-ul">
                <li>
                  <span class="fa-li"><i class="fa fa-check"></i></span
                  ><strong>Equipes compléte</strong>
                </li>
                <li>
                  <span class="fa-li"><i class="fa fa-check"></i></span>Weekend
                  acceptés
                </li>
                <li>
                  <span class="fa-li"><i class="fa fa-check"></i></span>24/7
                </li>
                <li>
                  <span class="fa-li"><i class="fa fa-check"></i></span>
                </li>
                <li>
                  <span class="fa-li"><i class="fa fa-check"></i></span>...
                </li>
                <li>
                  <span class="fa-li"><i class="fa fa-check"></i></span>...
                </li>
                <li>
                  <span class="fa-li"><i class="fa fa-check"></i></span
                  ><strong>Garantie de résultat</strong> ..
                </li>
                <li>
                  <span class="fa-li"><i class="fa fa-check"></i></span>...
                </li>
              </ul>
              <a href="#" class="btn btn-block btn-primary text-uppercase"
                >Commander</a
              >
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
section.pricing {
  margin-top: 50px;
  background: #129aab;
  background: linear-gradient(to right, #8acbbd, #129aab);
}

.pricing .card {
  border: none;
  border-radius: 1rem;
  transition: all 0.2s;
  box-shadow: 0 0.5rem 1rem 0 rgba(0, 0, 0, 0.1);
}

.pricing hr {
  margin: 1.5rem 0;
}

.pricing .card-title {
  margin: 0.5rem 0;
  font-size: 0.9rem;
  letter-spacing: 0.1rem;
  font-weight: bold;
}

.pricing .card-price {
  font-size: 3rem;
  margin: 0;
}

.pricing .card-price .period {
  font-size: 0.8rem;
}

.pricing ul li {
  margin-bottom: 1rem;
}

.pricing .text-muted {
  opacity: 0.7;
}

.pricing .btn {
  font-size: 80%;
  border-radius: 5rem;
  letter-spacing: 0.1rem;
  font-weight: bold;
  padding: 1rem;
  opacity: 0.7;
  transition: all 0.2s;
}

/* Hover Effects on Card */

@media (min-width: 992px) {
  .pricing .card:hover {
    margin-top: -0.25rem;
    margin-bottom: 0.25rem;
    box-shadow: 0 0.5rem 1rem 0 rgba(0, 0, 0, 0.3);
  }
  .pricing .card:hover .btn {
    opacity: 1;
  }
}
</style>
