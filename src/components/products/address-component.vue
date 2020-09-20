<template>
  <div :class=" $q.screen.sm || $q.screen.lt.sm
  ? 'row items-center justify-center' : 'row items-center'">
    <div class="col-md col-sm col-xs">
      <div class="q-ml-md row items-center" style="height:40px">
        <q-icon name="place" size="21px" />
        <p
          class="q-ma-sm text-weight-bold contact-info"
          :style="$q.screen.lt.xl ? 'font-size: 22px': ''"
        >
          <slot name="name" />
        </p>
      </div>
      <div class="q-ml-lg">
        <p
          class="text-weight-medium q-mb-none q-ml-lg"
          :style="$q.screen.lt.xl ? 'font-size: 18px': 'font-size: 19px'"
        >
          <slot name="street" />
        </p>
        <p class="q-ml-xl" style="font-size:15px">
          <slot name="city" />
        </p>
      </div>
    </div>
    <div :class="$q.screen.xl ? 'q-ml-lg': 'q-ml-lg col-xs-1 col-sm-1 col-md-1'">
      <q-btn flat icon="directions" @click="$emit('on-submit')" />
    </div>
    <div class="col-md-1 col-sm-2 col-xs-1" />
  </div>
</template>

<script>

export default {
  name: 'address-component',
};
</script>

<style scoped>
  .contact-info {
    font-size:25px;
    letter-spacing: 2px
  }
</style>
