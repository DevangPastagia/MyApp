<template>
    <div class="row">
        <div class="col-lg-8 col-md-8 col-sm-11 align-items-center">
            <MenusSlots>
                <template v-slot:menusgrid>
                    {{ menusgrid }}
                </template>
            </MenusSlots>
        </div>
        <div class="col-lg-4 col-md-4 col-sm-1">
            <a href="#" class="btn btn-primary rounded-0 filter float-end gap-2" data-bs-toggle="modal" data-bs-target="#staticBackdrop">
                <img src="@/assets/icons/Vector.png" alt="No Image">filter
            </a>

            <!-- Modal -->
            <div class="modal fade" id="staticBackdrop" data-bs-backdrop="static" data-bs-keyboard="false" tabindex="-1" aria-labelledby="staticBackdropLabel" aria-hidden="true">
                <div class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-header">
                    <h1 class="modal-title fs-5" id="staticBackdropLabel">Modal title</h1>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                    </div>
                    <div class="modal-body">
                        <MenusSlots>
                            <template v-slot:menusgrid>
                                {{ menusgrid }}
                            </template>
                        </MenusSlots>           
                    </div>
                    <div class="modal-footer">
                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Cancel</button>
                    <button type="button" class="btn btn-primary" data-bs-dismiss="modal">Filter</button>
                    </div>
                </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import MenusSlots from '../MenusSlots.vue';
export default {
  components: { MenusSlots },
    name:'TopGrid',
}
</script>