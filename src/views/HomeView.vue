<template>
  <div class="home">
    <TheCarusel />

    <TheFeauters :data="featureData" />
    <TheDoctors :data="doctorsData" />
    <TheСonsultationSignUp />

    <div class="home__slider">
      <CaruselPictureContent />
    </div>

  </div>
</template>



<script>
import { featureData, doctorsData } from '../data/data.rowThings';

import TheCarusel from '../components/TheCarusel.vue'
import TheFeauters from '../components/TheFeauters.vue'
import TheDoctors from '../components/TheDoctors.vue'
import TheСonsultationSignUp from '../components/TheСonsultationSignUp.vue'
import CaruselPictureContent from '../components/CaruselPictureContent.vue';

export default {
  name: 'HomeView',
  components: {
    TheCarusel,
    TheFeauters,
    TheDoctors,
    TheСonsultationSignUp,
    CaruselPictureContent,
  },

  data() {
    return {
      featureData: featureData,
      doctorsData: doctorsData,
    }
  }
}
</script>
