<template>
    <div class="row">
        <div class="col">
            <nav class="navbar navbar-expand-lg">
                <div class="offcanvas offcanvas-end" tabindex="-1" id="navbarOffcanvasLg" >
                    <div class="offcanvas-header">
                        <div class="offcanvas-title" id="offcanvasNavbarLabel">
                            <div class="d-flex justify-content-center align-items-center">
                                <img src="@/assets/logos/logo.png" alt="No Image">
                            </div>
                        </div>
                        <button type="button" class="btn-close btn-close-dark" data-bs-dismiss="offcanvas" aria-label="Close"></button>
                    </div>

                    <div class="offcanvas-body d-flex justify-content-center">
                        <ul class="navbar-nav flex-grow-1" >
                            <li class="nav-item " v-for="items in menus" :key="items.id">
                                <a class="nav-link active" aria-current="page" :href="`${items}`">{{ items }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </nav>
        </div>
    </div>
</template>

<script>
export default {
    name:'CategoryPart',
    data(){
        return{
            menus:["Jewelry & Accessories","Clothing & Shoes","Home & Living","Wedding & Party","Toy & Entertainment","Art & Collectibles","Craf Supplies & Tools"]
        }
    }
}
</script>