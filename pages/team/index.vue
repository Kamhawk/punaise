<template>
  <div class="premier-elem-page">
    <div class="container-md">
      <info-card
        :frontType="'graph'"
        :frontTitle="front.title"
        :frontData="front.graphData"
        :backTitle="back.title"
        :backData="back.message"
      />
      <vueFlashCard
        front="hello this is a flashcard"
        color-front="black"
        back="with animation"
      >
      </vueFlashCard>
    </div>
  </div>
</template>

<script>
import InfoCard from 'vue-info-card'
import vueFlashCard from 'vue-flashcard'

export default {
  components: {
    InfoCard,
    vueFlashCard
  },
  data() {
    return {
      front: {
        title: 'Amdy Diop',
        message:
          "Concernant l'implémentation de l'adaptabilité interne / externe, il faut performer les thématiques investissement.",
        data: [
          "Concernant l'implémentation de l'adaptabilité interne / externe, il faut performer les thématiques investissement."
        ]
      },
      back: {
        title: 'Engagements',
        message:
          "Concernant l'implémentation de l'adaptabilité interne / externe, il faut performer les thématiques investissement."
      }
    }
  }
}
</script>

<style scoped>
.premier-elem-page {
  padding-top: 200px;
  background-image: url('../../assets/landscape/homme-produit.jpg');
  background-size: cover;
  padding-bottom: 5px;
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-position: center;
}
</style>
