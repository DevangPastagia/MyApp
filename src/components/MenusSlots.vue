<template>
    <div>
        <slot :name="menusgrid">
            <ul class="nav nav-tabs border border-0">
                <li class="nav-item" v-for="menus in gridmenu" :key="menus">
                    <a v-if="gridmenu.indexOf(menus) == 0" class="nav-link active border-0" aria-current="page" href="#">{{ menus }}</a>
                    <a v-else class="nav-link border-0" aria-current="page" href="#">{{ menus }}</a>
                </li>
            </ul>
        </slot>
    </div>
</template>

<script>
import Category from '@/Mixins/MixCategory.vue';
export default {
    name: 'MenusSlots',
    mixins:[Category]
}
</script>