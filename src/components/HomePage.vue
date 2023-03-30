<template>
  <div>
    <div class="bg-white">
      <!-- banner Image -->
      <div class="overlay">
        <div id="imgBanner" class="imgBanner center mx-auto">
          <div class="gridinfo"></div>
          <img
            src="https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/hero-logo.png"
            alt=""
          />
        </div>
      </div>

      <!--Navbar  -->
      <!-- <nav class="navbar sticky-top bg-light N400 P200"> -->
      <Navbar />
      <!-- </nav> -->

      <!-- Who are we -->
      <WhoAreWe />

      <!-- count down timer -->
      <div class="countdown border center bg-light">
        <!-- <Countdown end="August 22, 2023"></Countdown> -->
      </div>

      <!-- about us -->
      <AboutUs/>
      

      <!-- when and where -->
      <WhenAndWhere/>
      

      <!-- map -->
      <div id="map" class="map py-10 center bg-light">
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3970.8364135748293!2d-0.32200338474948165!3d5.591178034848167!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0xfdfa3ced6d60fb5%3A0x7ba525d2f6eebb8e!2sLinda%20Dor%20Restaurant%20(Main)!5e0!3m2!1sen!2sgh!4v1679568284737!5m2!1sen!2sgh" width="10000rem" height="600" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>

      <!-- Gift Registry -->
      <div class="giftRegistry py-10 borde center">Gift Registry</div>

      <!-- RSVP -->
      <div id="rsvp" class="rsvp my-10 border center">
        <!-- <img src="https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/rsvp.jpg" width="1600" height="900" data-stellar-ratio="0.5" alt="" style="opacity: 1; transform: translate3d(0px, -128.409px, 0px); width: 1903px; height: 1070.44px; margin-top: -58.3827px; margin-left: 0px;"> -->
        <div class="container">
          <form action=""></form>
        </div>
      </div>

      <!-- Grooms and braidmaids -->
      <!-- <MenAndMaids/>
      <MenAndMaids/> -->

      <!-- Quotes -->
      <Quotes/>

      <!-- Photo Gallery -->
      <PhotoGallerySection/>

      <!-- Footer -->
      <!-- <FooterSection/> -->
      
    </div>
  </div>
</template>

<script>
import Navbar from './HomePageComp/Navbar.vue'
import AboutUs from './HomePageSection/AboutUs.vue'
import MenAndMaids from './HomePageSection/MenAndMaids.vue'
import Quotes from './HomePageSection/Quotes.vue'
import WhenAndWhere from './HomePageSection/WhenAndWhere.vue'
import WhoAreWe from './HomePageSection/WhoAreWe.vue'
import FooterSection from './HomePageSection/FooterSection.vue'
import PhotoGallerySection from './HomePageSection/PhotoGallerySection.vue'
import Countdown from 'vuejs-countdown'

export default {
  name: 'WeddingHomePage',
  data() {
    return {}
  },
  mounted() {},
  methods: {},
  components: { Countdown, Navbar, WhoAreWe, AboutUs, WhenAndWhere, MenAndMaids, Quotes, PhotoGallerySection, FooterSection }
}
</script>

<style >
@import url('https://fonts.googleapis.com/css2?family=Alex+Brush&display=swap');

.gridinfo {
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
  background: rgba(0,0,0,0.3);
  text-align: center;
  transition: all 0.8s;
}

/* Extra small devices (phones, 600px and down) */
@media only screen and (max-width: 600px) {
}

/* Small devices (portrait tablets and large phones, 600px and up) */
@media only screen and (min-width: 600px) {
}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {
}

/* Large devices (laptops/desktops, 992px and up) */
@media only screen and (min-width: 992px) {
    
}

/* Extra large devices (large laptops and desktops, 1200px and up) */
/* @media only screen and (min-width: 1200px) { */
  .center {
    justify-content: center;
    align-items: center;
    display: flex;
  }
  .imgBanner {
    height: 100vh;
    /* width: 100vw; */
    background-color: aqua;
    background-image: url(https://res.cloudinary.com/akwaah/image/upload/v1680203747/CG7A3084_ihsozw.jpg);
    background-repeat: no-repeat;
    background-size: cover;
  }
  .overlay {
    /* height: 100vh;
  width: 100vw; */
    background-color: aqua;
    z-index: 2;
  }
  .stickyNavbar {
    /* height: 7rem; */
    /* background-color: grey; */
  }
  .whoWeAre {
    /* height: 60vh; */
    /* background-color: red; */
  }
  .countdown {
    height: 10rem;
  }
  .aboutUs {
    /* height: 120vh; */
  }

  .brideGroomImage {
    /* height: 43.5vh; */
    background-repeat: no-repeat;
    background-size: contain;
    background-position: center center;
  }
  .whenNwhere {
    /* height: 90vh; */
  }
  .map {
    /* height: 60vh; */
  }
  .giftRegistry {
    height: 40vh;
  }

  .rsvp {
    height: 120vh;
    background-image: url(https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/rsvp.jpg);
    background-repeat: no-repeat;
    background-attachment: fixed;
    background-size: cover;
  }

  .avatar {
    /* width: 20rem;
    height: 20rem; */
  }

  .menAndMaids {
    /* height: 50vh; */
  }

  .quotes {
    height: 50vh;
    background-image: url(https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/quote.jpg);
    background-repeat: no-repeat;
    background-attachment: fixed;
    background-size: cover;
    font-style: italic;
  }

  .footer {
    /* height: 75vh; */
    background-image: url(https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/rsvp.jpg);
    background-repeat: no-repeat;
  }

  .footerImage {
    height: 5rem;
  }
/* } */
</style>
