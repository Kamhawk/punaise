<template>
  <div class="container premier-elem-page">
    <full-calendar :events="fcEvents" locale="en"></full-calendar>
  </div>
</template>

<script>
import fullCalendar from 'vue-fullcalendar'

const demoEvents = [
  {
    title: 'Sunny Out of Office',
    start: '2016-08-25',
    end: '2017-07-27'
  },
  {
    title: 'event1',
    start: '2016-07-01'
  },
  {
    title: 'event2',
    start: '2016-07-02',
    end: '2016-07-03'
  }
]
export default {
  name: 'Calendar',
  components: { fullCalendar },
  data() {
    return {
      fcEvents: demoEvents
    }
  }
}
</script>

<style scoped>
.premier-elem-page {
  padding-top: 100px;
}
</style>
