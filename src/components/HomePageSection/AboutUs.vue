<template>
    <div id="aboutUs" class="aboutUs  p-10 container bg-transparent" >
          <div class="borde text-center H900 N600 pb-10">Groom & Bride</div>

          <div class="row  ">
            <div
              class="col-md-6 col-lg-4  p-0 brideGroomImage "
              
            >
              <!-- <img src="https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/about-groom-540x405.jpg" alt="" srcset=""> -->
            </div>
            <div class="col-md-6 col-lg-8 my-auto p-10  ">
              <ProfileCard/>
            </div>
            <div class="col-md-6 col-lg-8  my-auto p-10 py-10 d-none d-md-block ">
                <ProfileCard/>
              
            </div>
            <div
              class=" col-md-6 col-lg-4 p-0   imageCover"
              
            >
            <!-- <img class="" src="https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/about-bride-540x405.jpg" alt="" srcset=""> -->
            </div>
            <div class="col-md-6 my-auto p-10 py-10 d-block d-md-none">
                <ProfileCard/>
              
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

<style scoped>

.brideGroomImage {
  background-image: url(https://res.cloudinary.com/akwaah/image/upload/v1680203721/CG7A3085_v2kbeh.jpg);
    height: 40vh;
    background-position: top center;
    background-repeat: no-repeat;
    background-size: cover;
    border: 0.1rem solid #b13a1a;
    border-radius: 5%;
    
}

.imageCover {
  background-image: url(https://res.cloudinary.com/akwaah/image/upload/v1680203699/CG7A3050_tvdisn.jpg);
    height: 40vh;
    background-position: top center;
    background-repeat: no-repeat;
    background-size: cover;
    border: 0.1rem solid #b13a1a;
    border-radius: 5%;
}

</style>