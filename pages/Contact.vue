<template>
  <!-- Contact Section -->
  <section id="contact" class="contact-section bg-secondary-custom">
    <div class="container">
      <div class="row">
        <div class="col-md-4 mb-3 mb-md-0">
          <div class="card py-4 h-100">
            <div class="card-body text-center">
              <i class="fa fa-map text-primary-custom mb-2"></i>
              <h4 class="text-uppercase m-0">Adresse</h4>
              <hr class="my-4" />
              <div class="small text-black-50">
                {{ localadress }}
              </div>
            </div>
          </div>
        </div>

        <div class="col-md-4 mb-3 mb-md-0">
          <div class="card py-4 h-100">
            <div class="card-body text-center">
              <i class="fa fa-envelope text-primary-custom mb-2"></i>
              <h4 class="text-uppercase m-0">Email</h4>
              <hr class="my-4" />
              <div class="small text-black-50">
                <a href="#">{{ localemail }}</a>
              </div>
            </div>
          </div>
        </div>

        <div class="col-md-4 mb-3 mb-md-0">
          <div class="card py-4 h-100">
            <div class="card-body text-center">
              <i class="fa fa-mobile text-primary-custom mb-2"></i>
              <h4 class="text-uppercase m-0">Mobile</h4>
              <hr class="my-4" />
              <div class="small text-black-50">{{ localmobile }}</div>
            </div>
          </div>
        </div>
      </div>
      <social-sharing url="https://vuejs.org/" inline-template>
        <div>
          <network network="facebook">
            <div class="container">
              <div class="row">
                <i class="fa fa-fw fa-facebook"></i>
              </div>
              <div class="row">
                Facebook
              </div>
            </div>
          </network>
          <network network="googleplus">
            <i class="fa fa-fw fa-google-plus"></i> Google +
          </network>
          <network network="linkedin">
            <i class="fa fa-fw fa-linkedin"></i> LinkedIn
          </network>
          <network network="pinterest">
            <i class="fa fa-fw fa-pinterest"></i> Pinterest
          </network>
          <network network="reddit">
            <i class="fa fa-fw fa-reddit"></i> Reddit
          </network>
          <network network="twitter">
            <i class="fa fa-fw fa-twitter"></i> Twitter
          </network>
          <network network="vk"> <i class="fa fa-vk"></i> VKontakte </network>
          <network network="weibo"> <i class="fa fa-weibo"></i> Weibo </network>
          <network network="whatsapp">
            <i class="fa fa-fw fa-whatsapp"></i> Whatsapp
          </network>
        </div>
      </social-sharing>
    </div>
  </section>
</template>

<script>
import SocialSharing from 'vue-social-sharing'
import { state } from '../store/constantes'

export default {
  name: 'Contact',
  components: { SocialSharing },
  data() {
    return {
      localmobile: state().mobile,
      localemail: state().email,
      localadress: state().adress
    }
  }
}
</script>

<style scoped>
.social-list-item {
  width: fit-content;
  color: yellow;
}
</style>
