<template>
    <carousel :autoplay="true" :nav="false" :dots="false" :items="4">
        <div class="card border-0" v-for="items in products" :key="items">
            <a href="#" class="text-decoration-none mx-1">
                <label v-if="items.tag && items.tag=='sale'" class="sale">{{ items.tag }}</label>
                <label v-if="items.tag && items.tag=='hot'" class="hot">{{ items.tag }}</label>
                <img :src="require(`@/assets/images/${items.image}`)" alt="No Image">
                <div class="card-body">
                    <h5 class="card-title">{{ items.name }}</h5>
                    <label class="float-start type">{{ items.type }}</label>
                    <div v-if="items.discount" class="float-end pricedisplay">
                        <div>
                            <label class="float-start price">
                                <s class="type">${{ items.price }}</s>
                            </label>
                            <label class="float-end price discount">${{ items.discount }}</label>
                        </div>
                    </div>

                    <div v-else class="float-end price d-flex gap-2">
                        <label class="float-end price">${{ items.price }}</label>
                    </div>
                </div>
            </a>
        </div>
    </carousel>
</template>
<script>
import MixCategory from '@/Mixins/MixCategory.vue';
import carousel from 'vue-owl-carousel'
export default {
    name:'CurouslSet',
    mixins:[MixCategory],
    components:{carousel},
}
</script>