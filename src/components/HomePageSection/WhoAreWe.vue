<template>
  <div id="whoWeAre" class="whoWeAre border p-10  center bg-white">
    
      <div class="row">
        <div class="col-md-5 mx-auto">
          <ProfileImage :whoarewe="groom"/>
        </div>
        <div class="col-md-2 py-xs-10 d-flex justify-content-center align-items-center">
          <img
            width="160"
            height="100"
            src="https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/intro-separator.png"
            alt=""
            loading="lazy"
          />
        </div>
        <div class="col-md-5">
          
          <ProfileImage :whoarewe="bride"/>
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
    return {
      groom : {
          id: 1,
          name: "Jojo Abbiw",
          photo: "https://res.cloudinary.com/akwaah/image/upload/v1680212991/Jojo_Akwaah_Abbiw_nlfvff.jpg"
        },
       bride: {
          id: 2,
          name: "Alberta Opoku-Mensah",
          photo: "https://res.cloudinary.com/akwaah/image/upload/v1680203748/CG7A3054_njkkvb.jpg"
        }
      
    }
  },

  mounted() {},

  methods: {}
}
</script>

<style lang="scss" scoped></style>
