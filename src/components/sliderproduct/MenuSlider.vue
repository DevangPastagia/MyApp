<template>

    <div class="row my-5">
        <div class="col-lg-8 col-md-8 col-sm-11 align-items-center">
            <MenusSlots>
                <template v-slot:menusgrid>
                    {{ menusgrid }}
                </template>
            </MenusSlots>
        </div>
        <div class="col-lg-4 col-md-4 col-sm-1">
            <a href="#" class="btn bg-primary btn-dark rounded-0 filter float-end gap-2 ">
                Show all
            </a>
        </div>
    </div>
</template>

<script>
import MenusSlots from '../MenusSlots.vue';
export default {
  components: { MenusSlots },
    name:'MenuSlider',
}
</script>