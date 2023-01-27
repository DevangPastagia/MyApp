<template>
  <div class="wrapper">
    <index/>
    <GoTo />
  </div>
</template>

<script>
import index from './view/index.vue';
import GoTo from './view/GoTo.vue';
export default {
  name: 'App',
  components: {
    index,
    GoTo
  },
};
</script>

<style>
@import '@/assets/css/style.css';
</style>
