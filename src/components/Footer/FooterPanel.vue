<template>
    <div class="footer">
        <div class="container top">
            <div class="row">
                <div class="col-sm-4">
                    <div class="left-footer d-flex justify-content-start align-items-center">
                        <img src="@/assets/logos/logo.png" alt="No Image">
                    </div>

                    <div class="mt-5 footer-content">
                        <p>
                            Lorem ipsum dolor sit amet, consectetur adipiscing
                            elit, sed do eiusmod tempor incididunt ut labore et
                            dolore magna aliqua
                        </p>
                    </div>

                    <div class="row social d-flex justify-content-start mt-5">
                        <div class="col-sm-3" v-for="items in social" :key="items.social">
                            <a href="#">
                                <img :src="require(`@/assets/icons/${items}`)" alt="No Image">                      
                            </a>
                        </div>
                    </div>
                </div>
                
                <div class="col-sm-3 foot-menu">
                    <h2 class="headings d-flexm justify-content-center align-items-center">
                        CATALOG
                    </h2>
                    <ul class="list-unstyled">
                        <li v-for="items in catelog" :key="items">
                          <a href="#!" class="text-decoration-none">{{ items }}</a>
                        </li>
                    </ul>              
                </div>
                
                <div class="col-sm-3 foot-menu">
                    <h2 class="headings d-flexm justify-content-center align-items-center">
                        ABOUT US
                    </h2>
                    <ul class="list-unstyled">
                        <li v-for="items in aboutus" :key="items">
                          <a href="#!" class="text-decoration-none">{{ items }}</a>
                        </li>
                    </ul>              
                </div>

                <div class="col-sm-2 foot-menu">
                    <h2 class="headings d-flexm justify-content-center align-items-center">
                        CUSTOMER SERVICES
                    </h2>
                    <ul class="list-unstyled">
                        <li v-for="items in customerservice" :key="items">
                          <a href="#!" class="text-decoration-none">{{ items }}</a>
                        </li>
                    </ul>              
                </div>
            </div>
        </div>

        <div class="container-fluid foot-end">
            <div class="container">
                <div class="row">
                    <div class="col-md-4">
                        © 2022 Coral , Inc.
                    </div>
                    <div class="col-md-4">
                        <img src="@/assets/images/icons_payment 1.png" alt="No Image">
                    </div>
                </div>
            </div>  
        </div>
    </div>
</template>

<script>
import MixCategory from '@/Mixins/MixCategory.vue';
export default {
    name: 'FooterPanel',
    mixins:[MixCategory]
}
</script>