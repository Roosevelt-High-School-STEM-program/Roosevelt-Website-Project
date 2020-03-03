<template>
  <div class="row bg-website-white" style="height:800px;">
    <div class="col-md-12"></div>
    <div
      class="col-md-12"
      style=""
    >
      <div
        class="row justify-center col-md-12"
      >
        <q-img
          transition="slide-right"
          style="width:460px; max-height:339px; border-radius: 25px 0px 0px 10px"
          :src="rotatingPictures"
        />
        <q-img
          style="width:460px; max-height:339px;"
          src="../../statics/rotating-photos/blueBerryPastries.jpeg"
        />
        <q-img
          style="width:460px; max-height:339px;"
          src="../../statics/rotating-photos/orangePastries.png"
        />
      </div>
      <div class="row justify-center col-md-12">
        <q-img
          style="width:460px; max-height:339px;"
          src="../../statics/rotating-photos/blueBerryPastries.jpeg"
        />
        <q-img
          style="width:460px; max-height:339px;"
          src="../../statics/rotating-photos/cookies.jpg"
        />
        <q-img
          style="width:460px; max-height:339px;"
          src="../../statics/rotating-photos/blueBerryPastries.jpeg"
        />

      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'RegularAboutPictures',
  data() {
    return {
      test1: '../../statics/rotating-photos/blueBerryPastries.jpeg',
      test2: '',
      idk: true,
      listOfPhotos: [
        '../../statics/rotating-photos/orangePastries.png',
        '../../statics/rotating-photos/blueBerryPastries.jpeg',
      ],
    };
  },
  computed: {
    rotatingPictures() {
      let photo = '../../statics/rotating-photos/cookies.jpg';
      // when page loads run the function
      // do a settimeout then switch photos
      // do another set timeout and switch out the photos again
      // for loop through the photos?
      // restart
      for (let i = 0; i < this.listOfPhotos.length; i += 1) {
        photo = this.listOfPhotos[i];
        // return photo;
      }
      console.log(photo);
      return photo;
    },
  },
  methods: {
  },
};
</script>

<style scoped>

</style>
