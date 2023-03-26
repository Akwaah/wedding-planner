<template>
  <div id="whoWeAre" class="whoWeAre border p-10  center">
    
      <div class="row">
        <div class="col-5 mx-auto">
          <ProfileImage />
        </div>
        <div class="col-2 d-flex justify-content-center align-items-center">
          <img
            width="160"
            height="100"
            src="https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/intro-separator.png"
            alt=""
            loading="lazy"
          />
        </div>
        <div class="col-5">
          
          <ProfileImage />
        </div>
 
      <div class="text-center mt-5">
        <p class="P400 N600" style="font-family: Alex Brush">Are getting married</p>
        <div class="P300 N600 mt-5">on 22 April, 2023 - Accra, Madina</div>
      </div>
    </div>
  </div>
</template>

<script>
import ProfileImage from '../HomePageComp/ProfileImage.vue'
export default {
  components: { ProfileImage },
  name: 'WeddingWhoAreWe',

  data() {
    return {}
  },

  mounted() {},

  methods: {}
}
</script>

<style lang="scss" scoped></style>
