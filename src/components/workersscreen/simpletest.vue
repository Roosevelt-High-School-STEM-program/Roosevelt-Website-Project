<template>
  <div class="row justify-center bg-website-white" style="min-height: 1500px">
    <div class="row justify-center items-center col-md-12">
      <div class="col-md-3" />
      <div class="col-md-6">
        <q-img src="../../statics/ohana.png" />
      </div>
      <div class="col-md-3" />
      <div class="col-md-6">
        <q-img
          style="background-position: center;  box-shadow: 5px 5px 5px grey;"
          :ratio="870/506"
          src="../../statics/people-photos/groupPic.jpeg"
        />
      </div>
    </div>

    <div class="col-md-12" />
    <div
      class="row col-md-10 justify-center"
      style="font-family: Alegreya Sans SC;"
    >
      <!--      <div-->
      <!--        class="col-md-9 q-mt-md row items-center bg-website-gray"-->
      <!--        style="border-radius: 200px 0px 0px 200px; height: 300px;"-->
      <!--      >-->
      <div>
        <div
          @mouseover="hover=true"
          @mouseleave="hover=false"
          class="col-2"
          :style="darkenImg"
        />
        <!--        <div class="column col-md-7" style="height:300px">-->
        <!--          <div class="col-md-3">-->
        <!--            <h1-->
        <!--              class="q-my-none q-ml-md text-weight-bolder text-center"-->
        <!--              style="font-size: 32px"-->
        <!--            >-->
        <!--              Worker-->
        <!--            </h1>-->
        <!--          </div>-->
        <!--          <div class="col-md-5">-->
        <!--            <p-->
        <!--              class="col-md-5 q-ml-md q-my-none q-ml-md"-->
        <!--              style="font-size: 19px; font-family: Inter;"-->
        <!--            >-->
        <!--              This worker is incredible. I'm truly amazed by their performance.-->
        <!--   This worker is incredible. I'm truly amazed by their performance. LIke truly wow-->
        <!--              This worker is incredible. I'm truly amazed by their performance.-->
        <!--              This worker is incredible. I'm truly amazed by their performance.-->
        <!--            </p>-->
        <!--          </div >-->
        <!--        </div>-->
      </div>
      <div class="col-1"/>
      <!--      <div class="column items-center">-->
      <!--        <div class="col-md-1 q-mt-md top-triangle"/>-->
      <!--        <div class="col-md-1 bottom-triangle" />-->
      <!--      </div>-->
      <!--      <div-->
      <!--        class="col-md-9 q-mt-md row items-center bg-website-gray"-->
      <!--        style="border-radius: 200px 0px 0px 200px; height: 300px"-->
      <!--      >-->
      <div>
        <q-img
          class="col-2"
          style="
          width: 300px;
          height: 300px;
          border-radius: 50%; border: solid 3px black; background-color: rgba(0, 0, 0, 0.6)"
          src="../../statics/people-photos/worker-2.jpeg"
        />
        <!--        <div class="column col-md-7" style="height:300px">-->
        <!--          <div class="col-md-3">-->
        <!--            <h1-->
        <!--              class="q-my-none q-ml-md text-weight-bolder text-center"-->
        <!--              style="font-size: 32px"-->
        <!--            >-->
        <!--              Worker-->
        <!--            </h1>-->
        <!--          </div>-->
        <!--          <div class="col-md-5">-->
        <!--            <p-->
        <!--              class="col-md-5 q-ml-md q-my-none q-ml-md"-->
        <!--              style="font-size: 19px; font-family: Inter;"-->
        <!--            >-->
        <!--              This worker is incredible. I'm truly amazed by their performance.-->
        <!-- This worker is incredible. I'm truly amazed by their performance. LIke truly wow-->
        <!--              This worker is incredible. I'm truly amazed by their performance.-->
        <!--              This worker is incredible. I'm truly amazed by their performance.-->
        <!--            </p>-->
        <!--          </div >-->
        <!--        </div>-->
      </div>
      <div class="col-1"/>
      <!--      <div class="column items-center">-->
      <!--        <div class="col-md-1 q-mt-md top-triangle"/>-->
      <!--        <div class="col-md-1 bottom-triangle" />-->
      <!--      </div>-->
      <!--      <div-->
      <!--        class="col-md-9 q-my-md row items-center bg-website-gray"-->
      <!--        style="border-radius: 200px 0px 0px 200px; height: 300px;"-->
      <!--      >-->
      <div>
        <q-img
          class="col-2"
          style="width: 300px; height: 300px; border-radius: 50%; border:solid 3px black"
          src="../../statics/people-photos/worker-3.jpeg"
        />
        <!--        <div class="column col-md-7" style="height:300px">-->
        <!--          <div class="col-md-3">-->
        <!--            <h1-->
        <!--              class="q-my-none q-ml-md text-weight-bolder text-center"-->
        <!--              style="font-size: 32px"-->
        <!--            >-->
        <!--              Worker-->
        <!--            </h1>-->
        <!--          </div>-->
        <!--          <div class="col-md-5">-->
        <!--            <p-->
        <!--              class="col-md-5 q-ml-md q-my-none q-ml-md"-->
        <!--              style="font-size: 19px; font-family: Inter;"-->
        <!--            >-->
        <!--              This worker is incredible. I'm truly amazed by their performance.-->
        <!-- This worker is incredible. I'm truly amazed by their performance. LIke truly wow-->
        <!--              This worker is incredible. I'm truly amazed by their performance.-->
        <!--              This worker is incredible. I'm truly amazed by their performance.-->
        <!--            </p>-->
        <!--          </div >-->
        <!--        </div>-->
      </div>
      <!--      <div class="column items-center">-->
      <!--        <div class="col-md-1 q-mt-md top-triangle" />-->
      <!--        <div class="col-md-1 bottom-triangle" />-->
      <!--      </div>-->
    </div>

  </div>

</template>

<script>
export default {
  name: 'simpletest',
  data() {
    return {
      hover: false,
      defaultImgWorker1: 'background-image:url("../../statics/people-photos/worker-1.jpeg"); background-size:cover;',
    };
  },
  computed: {
    darkenImg() {
      if (this.hover) {
        return 'background-image:url("../../statics/people-photos/worker-1.jpeg"); background-size:cover; background-position: center; width: 300px; height: 300px; border-radius: 50%; box-shadow: 5px 5px 5px grey; background-color: rgba(0, 0, 0, 0.6)';
      }
      return 'background-image:url("../../statics/people-photos/worker-1.jpeg"); background-size:cover; background-position: center; width: 300px; height: 300px; border-radius: 50%; box-shadow: 5px 5px 5px grey; background-color: rgba(0, 0, 0, 0.6)';
    },
  },
  methods: {
    floatingImages() {

    },
  },
};
</script>

<style scoped>

</style>
