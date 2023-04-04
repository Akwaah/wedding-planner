<template>
    <div id="aboutUs" class="aboutUs  p-10 container bg-transparent" >
          <div class="borde text-center H900 N600 pb-10">Groom & Bride</div>

          <div class="row  ">
            <div
              class="col-md-6 col-lg-4  p-0 brideGroomImage rounded-xl">
            <div class="gridinfo rounded-xl"></div>
              <!-- <img src="https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/about-groom-540x405.jpg" alt="" srcset=""> -->
            </div>
            <div class="col-md-6 col-lg-8 my-auto p-10  ">
              <ProfileCard :aboutUs="groom"/>
            </div>
            <div class="col-md-6 col-lg-8  my-auto p-10 py-10 d-none d-md-block ">
                <ProfileCard :aboutUs="bride"/>
              
            </div>
            <div
              class=" col-md-6 col-lg-4 p-0   imageCover rounded-xl">
              <div class="gridinfo rounded-xl"></div>
            <!-- <img class="" src="https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/about-bride-540x405.jpg" alt="" srcset=""> -->
            </div>
            <div class="col-md-6 my-auto p-10 py-10 d-block d-md-none">
                <ProfileCard :aboutUs="bride"/>
              
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
            groom: {
              name: "Jojo Abbiw",
            content: "Jojo possesses a tranquil demeanor, coupled with remarkable patience, kindness, and a good sense of humor. Interestingly, fate brought him together with his wife-to-be on a night when there was a power outage 'Dumsor' on Legon campus, a situation that ultimately turned out to be a stroke of luck for him. In short, 'Dumsor' did him good 😂. ",
            cssClassContent: "text-lg-end",
            cssClassImage: "float-lg-end"
            },
            bride: {
              name: "Alberta Opoku-Mensah",
            content: "Alberta is a warm and sociable individual who exudes kindness and empathy. Fate brought her together with her spouse-to-be on a fateful night when she had to resort to using PENSA Legon's generator to heat her soup due to a power outage in her hostel. Over the course of the past six years, they have nurtured their relationship and now wish to formalize their commitment to each other through marriage.",
            cssClassContent: "text-start",
            cssClassImage: ""
            },
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
  background-image: url(https://res.cloudinary.com/akwaah/image/upload/v1680553609/IMG_20220219_132754_2_jptrld.jpg);
    height: 50vh;
    background-position: top top;
    background-repeat: no-repeat;
    background-size: cover;
    border: 0.1rem solid #b13a1a;
    border-radius: 5%;
    
}

.imageCover {
  background-image: url(https://res.cloudinary.com/akwaah/image/upload/v1680460921/IMG_20220219_132815_cyggtu.jpg);
    height: 50vh;
    background-position: top center;
    background-repeat: no-repeat;
    background-size: cover;
    border: 0.1rem solid #b13a1a;
    border-radius: 5%;
}

</style>