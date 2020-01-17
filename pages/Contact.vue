<template>
  <!-- Contact Section -->
  <section id="contact" class="contact-section bg-black">
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

      <social-sharing
        url="https://vuejs.org/"
        title="The Progressive JavaScript Framework"
        description="Intuitive, Fast and Composable MVVM for building interactive interfaces."
        quote="Vue is a progressive framework for building user interfaces."
        hashtags="vuejs,javascript,framework"
        twitter-user="vuejs"
        inline-template
      >
        <div class="social d-flex justify-content-center">
          <div>
            <network network="email">
              <i class="fa fa-envelope"></i>Email
            </network>
          </div>
          <div>
            <network network="facebook">
              <i class="fa fa-facebook"></i>Facebook
            </network>
          </div>
          <div>
            <network network="googleplus">
              <i class="fa fa-google-plus"></i>Google+
            </network>
          </div>
          <div>
            <network network="linkedin">
              <i class="fa fa-linkedin"></i>LinkedIn
            </network>
          </div>
          <div>
            <network network="pinterest">
              <i class="fa fa-pinterest"></i>Pinterest
            </network>
          </div>
          <div>
            <network network="skype">
              <i class="fa fa-skype"></i>Skype
            </network>
          </div>
          <div>
            <network network="sms">
              <i class="fa fa-commenting-o"></i>SMS
            </network>
          </div>
          <div>
            <network network="telegram">
              <i class="fa fa-telegram"></i>Telegram
            </network>
          </div>
          <div>
            <network network="twitter">
              <i class="fa fa-twitter"></i>Twitter
            </network>
          </div>
          <div>
            <network network="whatsapp">
              <i class="fa fa-whatsapp"></i>Whatsapp
            </network>
          </div>
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

<style scoped></style>
