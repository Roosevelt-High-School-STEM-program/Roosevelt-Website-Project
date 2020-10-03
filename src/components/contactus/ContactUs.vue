<template>
  <div class="row text-white background-img">
    <div
      class="row col-md-12 col-xs-12 justify-center bg-website-white"
      :style="ResponsiveContactPageSize"
    >
      <div class="col-md-12 col-xs-12 row justify-center text-center">
        <div class="col-md-12" />
        <div :class="ResponsiveContactInfoTitle">
          <h1
            class="q-my-sm text-weight-medium no-hightlight"
            :style="ResponsiveContactInfoTitleStyle"
          >
            CONTACT INFO
          </h1>
        </div>
        <div class="col-md-8 col-sm-12 col-xs-12 col-lg-7 row">
          <div class="col-md-4 col-sm-4 col-xs-12">
            <div class="row justify-center items-center">
              <q-icon name="place" :size="ResponsiveIcon" />
              <p
                class="q-ma-sm text-weight-bold contact-info no-hightlight"
                :style="ResponsiveInformationTitle"
              >
                Address
              </p>
            </div>
            <p
              class="q-ma-sm text-weight-medium"
              :style="ResponsiveInformation"
            >
              523 Ahui St, Honolulu, HI 96813
            </p>
          </div>
          <div class="col-md-4 col-sm-4 col-xs-12">
            <div class="row justify-center items-center">
              <q-icon name="phone" :size="ResponsiveIcon" />
              <p
                class="q-ma-sm text-weight-bold contact-info no-hightlight"
                :style="ResponsiveInformationTitle"
              >
                Phone
              </p>
            </div>
            <p
              class="q-ma-sm text-weight-medium"
              :style="ResponsiveInformation"
            >
              (808) 596-8415
            </p>
          </div>
          <div class="col-md-4 col-sm-4 col-xs-12">
            <div class="row justify-center items-center">
              <q-icon name="img:../../statics/instagramGlyphLogo.png" :size="ResponsiveIcon" />
              <p
                class="q-ma-sm text-weight-bold contact-info no-hightlight"
                :style="ResponsiveInformationTitle"
              >
                Instagram
              </p>
            </div>
            <p
              class="q-ma-sm text-weight-medium"
              :style="ResponsiveInformation"
            >
              @OriginalHawaiiOatCake
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ContactUs',
  computed: {
    ResponsiveContactInfoTitleStyle() {
      return this.$q.screen.lt.sm ? 'font-size: 53px' : '';
    },
    ResponsiveContactInfoTitle() {
      return this.$q.screen.lt.sm || this.$q.screen.sm ? 'col-md-12 col-xs-12 row items-center justify-center' : 'col-md-12 col-xs-12';
    },
    ResponsiveInformation() {
      return this.$q.screen.lt.sm ? 'font-size:13px' : 'font-size: 17px';
    },
    ResponsiveInformationTitle() {
      return this.$q.screen.lt.sm ? 'font-size:17px' : '';
    },
    ResponsiveIcon() {
      return this.$q.screen.lt.sm ? '16px' : '20px';
    },
    ResponsiveContactPageSize() {
      return this.$q.screen.lt.sm ? 'height: 350px; background-color: rgba(20, 15, 15, 0.7);padding-bottom:30px' : 'height: 325px; background-color: rgba(20, 15, 15, 0.7);';
    },
  },
};
</script>

<style scoped>
 .contact-info {
   font-size:19px;
   letter-spacing: 2px
 }
  .background-img {
    background-image: url('../../statics/food-pictures/oatmeal.jpg');
    background-size:cover;
  }
  h1 {
    font-family: Alegreya Sans SC;
    letter-spacing: 2px;
    font-size:90px
  }
</style>
