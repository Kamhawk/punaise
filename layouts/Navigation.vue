<template>
  <div class="fixed-top custom-navbar">
    <b-navbar
      id="mainNav"
      toggleable="lg"
      toggle-class="custom-navbar"
      type="dark"
      variant="faded"
      class="custom-navbar"
    >
      <b-navbar-brand href="/#page-top"
        ><img
          src="@/assets/pictos/debana.svg"
          width="40px"
          class="d-inline-block align-top"
          alt="Kitten"
        />
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item href="/#about">Nous connaitre</b-nav-item>
          <b-nav-item href="/team">Notre équipe</b-nav-item>
          <b-nav-item href="/tarifs">Tarifs</b-nav-item>
          <b-nav-item href="/blog">Blog</b-nav-item>
          <b-nav-item href="/calendar">Calendrier</b-nav-item>
          <b-nav-item href="/#contact">Contact</b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-item-dropdown right>
            <!-- Using 'button-content' slot -->
            <template v-slot:button-content>
              <em>Connexion</em>
            </template>
            <b-dropdown-item href="#">Utilisateur</b-dropdown-item>
            <b-dropdown-item href="#">Se déconnecter</b-dropdown-item>
          </b-nav-item-dropdown>
          <div class="container">
            <a href="">
              <font-awesome-icon :icon="['fab', 'linkedin']" />
            </a>
            <a href="">
              <font-awesome-icon :icon="['fab', 'github']" />
            </a>
            <a href="">
              <font-awesome-icon :icon="['fab', 'facebook']" />
            </a>
            <a href="">
              <font-awesome-icon :icon="['fas', 'coffee']" />
            </a>
          </div>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<style scoped>
.navbar-dark .navbar-nav .nav-link {
  color: #1d2b4d;
}
.custom-navbar {
  background: #129aab;
  color: #1d2b4d;
  padding: 0.15rem;
}
</style>
