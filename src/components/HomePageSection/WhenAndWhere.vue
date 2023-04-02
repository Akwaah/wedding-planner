<template>
    <div class="bgColor2">
    <div id="whenNwhere" class="whenNwhere p-10 container ">
          <div class="text-center H900 N600 mb-10">When & Where</div>
          <div class="row g-3">
            <div class="col-md-6 col-12 pl-0 ">
              <div class=" justify-content-center">
                <!-- <img
                  src="https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/event-party-540x270.jpg"
                  alt=""
                /> -->
                <div class="center avatar borderColor  mx-auto rounded-circle" style="background: #d0edf5; ">
                  <Engagement/>
                </div>
                <div class="p-10                       
                 text-center">
                  <div class="P400 N700 py-2 text-capitalize">Engagement</div>
                  <div class="P200 N700 py-2 text-capitalize">
                    Friday, 21 April
                  </div>
                  <div class="P200 N700 py-2 text-capitalize">
                    10.00 AM — 12.00 PM
                  </div>
                  <div class="P200 N700 py-2 text-capitalize">
                    Mr. Opoku-mensah's Residence
                  </div>
                  <div class="P200 N700 py-2 text-capitalize">
                    Bunso, Eastern Region
                  </div>
                  <div class="P200 N700 py-2 text-capitalize" style="color: #b13a1a">
                    0542163503
                  </div>
                  <button v-if="false" @click="setWeddingLoc(false, true)" type="button" class="btn bgColor2 borderColor py-2 text-capitalize" style="color: #b13a1a">See Map</button>
                </div>
              </div>
            </div>

            <div class="col-md-6 col-12 pr-0">
              <div class=" justify-content-center">
                <div class="center avatar borderColor  mx-auto rounded-circle" style="background: #d0edf5; ">
                  <Church/>
                </div>
                <div class="p-10                       
                 text-center">
                  <div class="P400 N700 py-2 text-capitalize">Wedding</div>
                  <div class="P200 N700 py-2 text-capitalize">
                    Saturday, 22 April
                  </div>
                  <div class="P200 N700 py-2 text-capitalize">
                    9.00 AM — 12.00 PM
                  </div>
                  <div class="P200 N700 py-2 text-capitalize">
                    Church of Pentecost, Fire Stone Worship Center
                  </div>
                  <div class="P200 N700 py-2 text-capitalize">
                    Madina, Greater Accra Region
                  </div>
                  <div class="P200 N700 py-2 text-capitalize" style="color: #b13a1a">
                    055353241/ 0246297177
                  </div>
                  <button v-if="false" @click="setWeddingLoc(true, false)" type="button" class="btn bgColor2 borderColor py-2 text-capitalize" style="color: #b13a1a">See Map</button>
                </div>
              </div>
              
            </div>
          </div>
          
      </div>
      <!-- map -->
      <div id="map" class="map py-10 center bgColor boderAroundT">
            <iframe v-if="this.showEngagementLoc" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3970.8364135748293!2d-0.32200338474948165!3d5.591178034848167!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0xfdfa3ced6d60fb5%3A0x7ba525d2f6eebb8e!2sLinda%20Dor%20Restaurant%20(Main)!5e0!3m2!1sen!2sgh!4v1679568284737!5m2!1sen!2sgh" width="10000rem" height="600" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
            <iframe v-if="this.showWeddingLoc" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d4721.509825572922!2d-0.17386632678151348!3d5.669592562469282!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0xfdf9ceb83c0bed1%3A0x887f679889627d5b!2sThe%20Church%20Of%20Pentecost%2C%20Firestone%20Worship%20Centre!5e0!3m2!1sen!2sgh!4v1680373067390!5m2!1sen!2sgh" width="100%" height="600" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>
    </div>
</template>

<script>
import Church from '../icons/church.vue';
import church from '../icons/church.vue';
import Engagement from '../icons/engagement.vue';
export default {
  components: { church, Church, Engagement },
    name: 'WeddingWhenAndHere',

    data() {
        return {
          showEngagementLoc: '',
          showWeddingLoc: ''
        };
    },

    mounted() {
        
    },

    methods: {
    setWeddingLoc ( wedding, engagement) { 
      showWeddingLoc = wedding
      showEngagementLoc = engagement
    },
    setEngagementLoc () {
      showEngagementLoc = true
      showWeddingLoc = false
    },
        
    },
    computed: {
      
    }
};
</script>

<style scoped>
.avatar {
        width: 10rem;
        height: 10rem;
        
      }
</style>