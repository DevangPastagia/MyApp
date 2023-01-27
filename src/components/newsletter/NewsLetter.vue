<template>
        <div class="container-fluid newsletter">
            <div class="container py-5">
                <h2 class="title-grid">Follow products and discounts on Instagram</h2>
                <div class="row mt-5 d-flex">
                    <div class="col-sm-2" v-for="items in newsletter" :key="items">
                        <div class="card rounded-0">
                            <div class="card-img-top">
                                <img :src="require(`@/assets/images/${items}`)" alt="No Image">
                                <div class="overlay">
                                    <div class="content">
                                        <img src="@/assets/icons/Vector-insta.png" alt="No Image">
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <h2 class="title-grid">Or subscribe to the newsletter</h2>
                <div class="d-flex justify-content-center mt-5 gap-3">
                    <input type="text" class="form-control w-50" placeholder="email address...">
                    <button class="btn">SUBMIT</button>
                </div>
            </div>
        </div>
</template>
<script>

import MixCategory from '@/Mixins/MixCategory.vue';
export default {
    name:'NewsLetter',
    mixins:[MixCategory]
}
</script>