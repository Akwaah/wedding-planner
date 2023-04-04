<template>
  <div id="whoWeAre" class="whoWeAre p-10  center bg-w boderAroundT" style="">
    
      <div class="row">
        <div class="col-md-5 mx-auto">
          <ProfileImage :whoarewe="groom"/>
          
        </div>
        <div class="col-md-2 py-xs-10 d-flex justify-content-center align-items-center">
          <img
            width="320"
            height="200"
            src="https://res.cloudinary.com/akwaah/image/upload/v1680436118/Untitled-1_mzqug3.png"
            alt=""
            loading="lazy"
          />
          

          <!-- <div class="H900 " style="font-size: 8rem; width:160;
            height:100;">
            &
          </div> -->
        </div>
        <div class="col-md-5">
          
          <ProfileImage :whoarewe="bride"/>
        </div>
 
      <div class="text-center mt-5">
        <p class="P400 N900" style="font-family: Alex Brush">Are getting married</p>
        <div class="P300 N900 mt-5">on 22 April, 2023 - Accra, Madina</div>
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
    return {
      groom : {
          id: 1,
          name: "Jojo Akwaah Abbiw",
          photo: "https://res.cloudinary.com/akwaah/image/upload/v1680644493/_MG_56081_aq567q.jpg"
        },
       bride: {
          id: 2,
          name: "Alberta Opoku-Mensah",
          photo: "https://res.cloudinary.com/akwaah/image/upload/v1680553608/IMG_8603_crcce5.jpg"
        }
      
    }
  },

  mounted() {},

  methods: {}
}
</script>

<style lang="scss" scoped></style>
