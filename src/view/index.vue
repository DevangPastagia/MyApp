<template>
    <div>
        <TopHeader/>
        <BrandLayout/>
        <HotCategory/>
        <GridProduct />
        <BannerPart />
        <SliderProduct />
        <NewsLetter />
        <FooterPanel />
    </div>
</template>

<script>
import TopHeader from '@/components/header/TopHeader/TopHeader.vue';
import BrandLayout from '@/components/brands/BrandLayout.vue';
import HotCategory from '@/components/hotcategory/HotCategory.vue';
import GridProduct from '@/components/gridproducts/GridProducts.vue'
import BannerPart from '@/components/banner/BannerPart.vue';
import SliderProduct from '@/components/sliderproduct/SliderProduct.vue';
import NewsLetter from '@/components/newsletter/NewsLetter.vue';
import FooterPanel from '@/components/Footer/FooterPanel.vue';
export default {
    name:'IndexPage',
    components:{
        TopHeader,
        BrandLayout,
        HotCategory,
        GridProduct,
        BannerPart,
        SliderProduct,
        NewsLetter,
        FooterPanel,
    }

}
</script>