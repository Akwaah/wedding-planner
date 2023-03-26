<template>
    <div id="aboutUs" class="aboutUs  p-10 container">
          <div class="borde text-center P400 N600 pb-10">Groom & Bride</div>
          <div class="row bg-light ">
            <div
              class="col-6  p-0 brideGroomImage d-flex justify-content-center"
              
            >
              <img src="https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/about-groom-540x405.jpg" alt="" srcset="">
            </div>
            <div class="col-6 my-auto p-10">
              <ProfileCard/>
            </div>
            <div class="col-6 my-auto p-10">
                <ProfileCard/>
              
            </div>
            <div
              class="col-6 p-0  brideGroomImage "
              
            >
            <img src="https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/about-bride-540x405.jpg" alt="" srcset="">
            </div>
          </div>
      </div>
</template>

<script>
import ProfileCard from '../HomePageComp/ProfileCard.vue';
export default {
  components: { ProfileCard },
    name: 'WeddingAboutUs',

    data() {
        return {
            
        };
    },

    mounted() {
        
    },

    methods: {
        
    },
};
</script>

<style lang="scss" scoped>

</style>