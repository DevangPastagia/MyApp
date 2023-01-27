<template>
    <div class="container-fluid d-flex justify-content-center align-items-center text-center my-5">
        <div class="container brand ">
            <div class="row">
                <div class="col" v-for="image in images" :key="image">
                    <a href="#">
                        <img :src="require(`@/assets/brands/${image}`)" alt="No Image">                      
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'BrandLayout',
    data(){
        return{
            images:['brand-1.png','brand-2.png','brand-3.png','brand-4.png','brand-5.png']
        }
    }
}
</script>