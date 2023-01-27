<template>
    <div class="container grid-product my-5">
        <h2 class="title-grid-product d-flex justify-content-center">new products</h2>
        <TopGrid />
        <Products />
    </div>
</template>

<script>
import TopGrid from './TopGrid.vue';
import Products from './Products.vue';
export default {
    name: 'GridProducts',
    components:{TopGrid,Products}
}
</script>