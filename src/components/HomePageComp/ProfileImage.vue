<template>
  <div class="">
    <img
      class="avatar mx-auto rounded-circle"
      :src='whoarewe.photo'
      alt="Rounded avatar"
    />
    <div class="P300 N600 text-center mt-5">{{ whoarewe.name }}</div>
  </div>
</template>

<script>
export default {
  props: {
   whoarewe: {
    id: Number,
    photo: String,
    name: String
   },
   
  },
  name: 'WeddingProfileImage',

  data() {
    return {}
  },

  mounted() {},

  methods: {}
}
</script>

<style scoped>
.avatar {
    width: 15rem;
    height: 15rem;
    border: 0.1rem solid #b13a1a;
  }
</style>
