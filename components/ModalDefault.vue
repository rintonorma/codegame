<template>
  <div class="modal fade" id="modalDefault" tabindex="-1" aria-labelledby="modalDefaultLabel" aria-hidden="true">
    <div class="modal-dialog modal-dialog-scrollable">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title"><slot name="modal-title"></slot></h5>
          <slot name="modal-close">
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close" @click="$emit('close')">
              <!-- <Icon icon="bi:x" height="24px"/> -->
            </button>
          </slot>
        </div>
        <div class="modal-body">
          <slot name="modal-content"></slot>
        </div>
        <div class="modal-add">
          <slot name="optional"></slot>
        </div>
        <div class="modal-footer">
          
          <slot name="modal-cta"></slot>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { Icon } from '@iconify/vue2';
export default {
  
  name: 'ModalDefault',
  components: {
    Icon
  },
  data () {
    return {

    }
  },
  
}
</script>

<style lang="scss" scoped>
.modal-title{
  text-transform: uppercase;
}
@media (max-width: 767px){
  .modal-dialog-scrollable{
    margin: 0;
    height: 100vh;
  }
  .modal-content{
    height: 100vh;
    border: 0;
    border-radius: 0;
  }
}
</style>
