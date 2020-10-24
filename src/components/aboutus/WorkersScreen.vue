<template>
  <div class="row justify-center bg-white q-mb-lg">
    <div class="row justify-center col-md-12 col-xs-12 q-my-md">
      <q-img class="col-md-3 col-xs-8 col-sm-5 q-mt-md" src="../../statics/Ohana2.png" />
      <div class="col-12"></div>
      <div class="col-md-7 col-xs-11 q-my-lg">
        <q-img
          class="float-image"
          style="background-position: center;"
          :ratio="870/506"
          src="../../statics/people-photos/groupPic.jpeg"
        />
      </div>
    </div>

    <div class="col-md-12 q-mt-lg" />
    <div class="row col-lg-10 col-sm-12 col-xs-12 justify-center worker-headers">
      <div
        class="col-lg-12 col-xs-10 col-sm-9 row justify-center items-center"
        style="min-height:360px"
      >
        <q-img
          :class="$q.screen.sm || $q.screen.lt.sm ? 'smaller-worker-image' : 'worker-image'"
          src="../../statics/people-photos/worker-1.jpeg"
        />
        <div class="offset-lg-1 col-lg-7 col-sm-12 col-xs-12 q-mb-lg">
          <div :class="$q.screen.sm || $q.screen.lt.sm ? 'q-my-sm' : 'q-my-lg q-ml-md'">
            <h1
              class="q-my-none text-weight-bolder text-center"
              :style="$q.screen.sm || $q.screen.lt.sm
               ? 'font-size: 25px; height:80px': 'font-size: 32px'"
            >
              First Name Last Name
            </h1>
            <p class="text-center">Years Worked</p>
          </div>
          <p
            class="q-ml-sm q-mt-md anaheim"
            :style="$q.screen.lt.sm ? 'font-size: 17px;' : 'font-size: 19px;'"
          >
            This worker is incredible. I'm truly amazed by their performance.
            This worker is incredible. I'm truly amazed by their performance. LIke truly wow
            This worker is incredible. I'm truly amazed by their performance.
            This worker is incredible. I'm truly amazed by their performance.
          </p>
        </div>
      </div>
      <div
        class="col-lg-12 col-xs-10 col-sm-9 row justify-center items-center"
        style="min-height:360px"
      >
        <div class="offset-lg-1 col-lg-7 col-sm-12 col-xs-12 q-mb-lg">
          <div :class="$q.screen.sm || $q.screen.lt.sm ? 'q-my-sm' : 'q-my-lg q-ml-md'">
            <h1
              class="q-my-none text-weight-bolder text-center"
              :style="$q.screen.sm || $q.screen.lt.sm
               ? 'font-size: 25px; height:80px': 'font-size: 32px'"
            >
              First Name Last Name
            </h1>
            <p class="text-center">Years Worked</p>
          </div>
          <p
            class="q-ml-sm q-mt-md anaheim"
            :style="$q.screen.lt.sm ? 'font-size: 17px;' : 'font-size: 19px;'"
          >
            This worker is incredible. I'm truly amazed by their performance.
            This worker is incredible. I'm truly amazed by their performance. LIke truly wow
            This worker is incredible. I'm truly amazed by their performance.
            This worker is incredible. I'm truly amazed by their performance.
          </p>
        </div>
        <q-img
          :class="$q.screen.sm || $q.screen.lt.lg
          ? 'smaller-worker-image order-first' : 'worker-image offset-lg-1 '"
          src="../../statics/people-photos/worker-2.jpeg"
        />
      </div>
      <div
        class="col-lg-12 col-xs-10 col-sm-9 row justify-center items-center"
        style="min-height:360px"
      >
        <q-img
          :class="$q.screen.sm || $q.screen.lt.sm ? 'smaller-worker-image' : 'worker-image'"
          src="../../statics/people-photos/worker-3.jpeg"
        />
        <div class="offset-lg-1 col-lg-7 col-sm-12 col-xs-12">
          <div :class="$q.screen.sm || $q.screen.lt.sm ? 'q-my-sm' : 'q-my-lg q-ml-md'">
            <h1
              class="q-my-none text-weight-bolder text-center"
              :style="$q.screen.sm || $q.screen.lt.sm
               ? 'font-size: 25px; height:80px': 'font-size: 32px'"
            >
              First Name Last Name
            </h1>
            <p class="text-center">Years Worked</p>
          </div>
          <p
            class="q-ml-sm q-mt-md anaheim"
            :style="$q.screen.lt.sm ? 'font-size: 17px;' : 'font-size: 19px;'"
          >
            This worker is incredible. I'm truly amazed by their performance.
            This worker is incredible. I'm truly amazed by their performance. LIke truly wow
            This worker is incredible. I'm truly amazed by their performance.
            This worker is incredible. I'm truly amazed by their performance.
          </p>
        </div>
      </div>
    </div>
  </div>

</template>

<script>
export default {
  name: 'RegularWorkersScreen',
};
</script>

<style scoped>
  .worker-image {
    width: 300px;
    height: 360px;
    box-shadow: 5px 5px 5px grey;
  }
  .smaller-worker-image {
    width: 250px;
    height: 310px;
    box-shadow: 5px 5px 5px grey;
  }
  .worker-description {

    font-family: 'Anaheim'
  }
</style>
