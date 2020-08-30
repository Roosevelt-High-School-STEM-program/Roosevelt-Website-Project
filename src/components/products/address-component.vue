<template>
  <div class="row items-center">
    <div>
      <div class="q-ml-md row items-center" style="height:40px">
        <q-icon name="place" size="22px" />
        <p class="q-ma-sm text-weight-bold contact-info">
          <slot name="place">
          </slot>
        </p>
      </div>
      <div class="q-ml-lg">
        <p class="text-weight-medium q-mb-none q-ml-lg" style="font-size: 20px">
          <slot name="address">
          </slot>
        </p>
        <p class="q-ml-xl" style="font-size:15px">
          <slot name="city">
          </slot>
        </p>
      </div>
    </div>
    <div :class="$q.screen.xl ? 'q-ml-xl': 'q-ml-lg'"><q-btn flat icon="directions"></q-btn></div>
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
