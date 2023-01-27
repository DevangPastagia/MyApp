<template>
    <div class="conteiner-fluid top-main bg-success">
        <div class="container p-3">
            <div class="row d-flex align-items-center">

                <!-- Search icon -->
                <div class="col-lg-4 col-md-6 searchbar d-flex justify-content-start align-items-center">
                    <a href="#">
                        <img src="@/assets/icons/search.png" alt="No Image" class="top-search" />
                    </a>
                    <div class="top-input">
                        <input type="text" class="form-control top-input rounded-pill" placeholder="Search product...">
                    </div>
                </div>

                <!-- Logo icon -->
                <div class="col-lg-4 col-md-6 d-flex justify-content-center">
                    <div>
                        <img src="@/assets/logos/logo.png" class="logo" alt="No Image"/>
                    </div>
                </div>

                <!-- Accounts -->
                <div class="col-lg-4 col-md-12 d-flex justify-content-end align-items-center">
                    <a href="#" class="text-decoration-none header-text d-flex align-item-center mx-3">
                        <img src="@/assets/icons/User.png" alt="No Image">Account
                    </a>
                    <a href="#" class="text-decoration-none header-text d-flex align-item-center">
                        <img src="@/assets/icons/Bag_alt.png" alt="No Image">Shopping
                    </a>

                    <nav class="navbar navbar-expand-lg d-flex justify-content-end mx-3">
						<button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#navbarOffcanvasLg" aria-controls="navbarOffcanvasLg">
							<span class="navbar-toggler-icon"></span>
						</button>
					</nav>
                </div>
            </div>

            <!-- horrizontal line -->
            <hr class="hr">

            <!-- Categories -->
            <Category/>
        </div>

        <!-- Top Main Content -->
        <TopMain />
    </div>
</template>

<script>
import TopMain from '@/components/header/TopMain.vue';
import Category from './Category.vue';

export default {
    name:'TopHeader',
    components:{TopMain,Category}

}
</script>