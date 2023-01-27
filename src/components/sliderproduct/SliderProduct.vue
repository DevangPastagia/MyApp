<template>
    <div class="container slider-product my-5">
        <h2 class="title-slider-product d-flex justify-content-center" >Best Sellers</h2>
        <MenuSlider />
        <Curousel />
    </div>
</template>

<script>
import MenuSlider from './MenuSlider.vue';
import Curousel from './Curousel.vue'
export default {
    name: "SliderProoduct",
    components: {MenuSlider,Curousel},
}
</script>