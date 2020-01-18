<template>
  <div>
    <Navigation />
    <nuxt />
    <Footer />
  </div>
</template>

<script>
import AOS from 'aos'
import Navigation from './Navigation'
import Footer from './Footer'
export default {
  components: { Navigation, Footer },
  beforeCreate() {
    AOS.init()
  }
}
</script>
