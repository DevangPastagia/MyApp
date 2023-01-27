<template>
    <div class="row cards-img">

        <div class="col-md-3" v-for="items in products" :key="items.name">
            <div class="card rounded-0 border-0">
                <div class="card-img-top">
                    <label v-if="items.tag && items.tag=='sale'" class="sale">{{ items.tag }}</label>
                    <label v-if="items.tag && items.tag=='hot'" class="hot">{{ items.tag }}</label>
                    <img :src="require(`@/assets/images/${items.image}`)" alt="No Image"/>
                    <div class="overlays">
                        <div class="contents d-flex justify-content-between align-items-center">
                            <a href="#"><img src="@/assets/icons/Favorite.png" alt="No Image" class="vectore-15"></a>
                            <a href="#"><img src="@/assets/icons/Group 64.png" alt="No Image" class="search"></a>
                            <a href="#" class="d-flex shopnow text-decoration-none justify-content-center align-items-center gap-2">
                                <img src="@/assets/icons/Bag_alt (1).png" alt="No Image" class="bag">
                                Shop now
                            </a>
                        </div>
                    </div>
                </div>
                <div class="card-body">
                    <h5 class="card-title">{{ items.name }}</h5>
                    <label class="float-start type">{{ items.type }}</label>
                    <div v-if="items.discount" class="float-end price d-flex gap-2">
                        <label class="float-start price">
                            <s class="type">${{ items.price }}</s>
                        </label>
                        <label class="float-end price discount">${{ items.discount }}</label>
                    </div>

                    <div v-else class="float-end price d-flex gap-2">
                        <label class="float-end price">${{ items.price }}</label>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import MixCategory from '@/Mixins/MixCategory.vue';
export default {
    name:'PrdouctsPart',
    mixins:[MixCategory]
}
</script>