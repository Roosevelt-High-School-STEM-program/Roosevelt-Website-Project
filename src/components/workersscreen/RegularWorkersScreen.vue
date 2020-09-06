<template>
  <div class="row justify-center bg-white q-pb-lg">
    <div class="row justify-center items-center col-md-12 q-my-md">
      <div class="col-md-3" />
      <div class="col-md-3 q-mt-md">
        <q-img src="../../statics/Ohana2.png" />
      </div>
      <div class="col-md-3" />
      <div class="col-md-7 q-my-lg">
        <q-img
          style="background-position: center; box-shadow: 5px 5px 5px grey;"
          :ratio="870/506"
          src="../../statics/people-photos/groupPic.jpeg"
        />
      </div>
    </div>

    <div class="col-md-12 q-mt-lg" />
    <div
      class="row col-md-10 justify-center worker-headers"
    >
      <div
        class="col-md-12 q-my-lg row items-center"
        style="height:360px"
      >
        <q-img
          class="worker-image"
          src="../../statics/people-photos/worker-1.jpeg"
        />
        <div class="col-md-7 offset-1" style="height:360px">
          <div class="q-my-lg q-ml-md">
            <h1
              class="q-my-none text-weight-bolder text-center"
              style="font-size: 32px"
            >
              First Name Last Name
            </h1>
            <p class="text-center">Years Worked</p>
          </div>
          <div>
            <p
              class="col-md-5 q-ml-md q-mt-md worker-description"
            >
              This worker is incredible. I'm truly amazed by their performance.
              This worker is incredible. I'm truly amazed by their performance. LIke truly wow
              This worker is incredible. I'm truly amazed by their performance.
              This worker is incredible. I'm truly amazed by their performance.
            </p>
          </div >
        </div>
      </div>
      <div
        class="col-md-12 q-mt-lg row items-center"
        style="height:360px"
      >
        <div class="col-md-7 offset-1" style="height:360px">
          <div class="q-my-lg q-ml-md">
            <h1
              class="q-my-none text-weight-bolder text-center"
              style="font-size: 32px"
            >
              First Name Last Name
            </h1>
            <p class="text-center">Years Worked</p>
          </div>
          <div>
            <p
              class="col-md-5 q-mt-md q-ml-md worker-description"
            >
              This worker is incredible. I'm truly amazed by their performance.
              This worker is incredible. I'm truly amazed by their performance. LIke truly wow
              This worker is incredible. I'm truly amazed by their performance.
              This worker is incredible. I'm truly amazed by their performance.
            </p>
          </div >
        </div>
        <q-img
          class="q-ml-md offset-1 worker-image"
          src="../../statics/people-photos/worker-2.jpeg"
        />
      </div>
      <div
        class="col-md-12 q-my-lg row items-center"
        style="height:360px"
      >
        <q-img
          class="worker-image"
          src="../../statics/people-photos/worker-3.jpeg"
        />
        <div class="col-md-7 offset-1" style="height:360px">
          <div class="q-my-lg q-ml-md">
            <h1
              class="q-my-none text-weight-bolder text-center"
              style="font-size: 32px"
            >
              First Name Last Name
            </h1>
            <p class="text-center">Years Worked</p>
          </div>
          <div>
            <p
              class="col-md-5 q-ml-md q-mt-md worker-description"
            >
              This worker is incredible. I'm truly amazed by their performance.
              This worker is incredible. I'm truly amazed by their performance. LIke truly wow
              This worker is incredible. I'm truly amazed by their performance.
              This worker is incredible. I'm truly amazed by their performance.
            </p>
          </div >
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
  .worker-description {
    font-size: 19px;
    font-family: 'Anaheim'
  }
  .worker-headers {
    font-family: Alegreya Sans SC;
  }
</style>
