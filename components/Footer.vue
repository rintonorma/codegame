<template>
  <div>
    <section>
      <div class="container">
        <h5 class="text-secondary mb-2 card-subtitle">DUKUNGAN PELANGGAN</h5>
        <h2 class="fw-bold mb-4 card-title">Hubungi kami</h2>
        <div class="row">
          <div class="col-6 col-lg-2 mb-3">
            <nuxt-link to="" class="text-dark">
              <div class="card border-0 rounded shadow p-4">
                <div class="d-flex align-items-center flex-column gap-2">
                  <Icon icon="logos:whatsapp" height="52px"/>
                  <div>Whatsapp</div>
                </div>
              </div>
            </nuxt-link>
          </div>
          <div class="col-6 col-lg-2 mb-3">
            <nuxt-link to="" class="text-dark">
              <div class="card border-0 rounded shadow p-4">
                <div class="d-flex align-items-center flex-column gap-2">
                  <Icon icon="dashicons:email" height="52px" class="text-danger"/>
                  <div>Email</div>
                </div>
              </div>
            </nuxt-link>
          </div>
          <div class="col-6 col-lg-2 mb-3">
            <nuxt-link to="" class="text-dark">
              <div class="card border-0 rounded shadow p-4">
                <div class="d-flex align-items-center flex-column gap-2">
                  <Icon icon="fluent:chat-help-24-filled" height="52px" class="text-danger"/>
                  <div>FAQ</div>
                </div>
              </div>
            </nuxt-link>
          </div>
          <div class="col-6 col-lg-2 mb-3">
            <nuxt-link to="" class="text-dark">
              <div class="card border-0 rounded shadow p-4">
                <div class="d-flex align-items-center flex-column gap-2">
                  <Icon icon="si-glyph:customer-support" height="52px" class="text-danger"/>
                  <div>Hotline</div>
                </div>
              </div>
            </nuxt-link>
          </div>
        </div>
      </div>  
    </section>
    <section class="bg-light">
      <div class="container footer-sub">
        <div class="mb-4"><img src="~/static/img/logo.svg" height="25px"></div>
        <div class="row">
          <div class="col-12 col-lg-4 mb-3"><small>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam volutpat risus suscipit dolor. Quis aliquam convallis amet, rhoncus etiam sapien sed lacus. Commodo fusce malesuada imperdiet amet convallis massa enim vivamus vestibulum. Iaculis sagittis pulvinar amet, potenti aliquam neque, risus purus. Habitant adipiscing sollicitudin vitae augue urna arcu blandit diam. Urna in in suspendisse magna. Dui, vitae ultrices lectus nunc sit nec.</small></div>
          <div class="col-12 col-lg-8 footer-menu">
            <ul class="">
              <li><nuxt-link to="" class="btn-link text-dark">Pemasaran dan Kemitraan</nuxt-link></li>
              <li><nuxt-link to="" class="btn-link text-dark">Syarat & Ketentuan</nuxt-link></li>
              <li><nuxt-link to="" class="btn-link text-dark">Kebijakan & Privasi</nuxt-link></li>
              <li><nuxt-link to="" class="btn-link text-dark">Berita & Acara</nuxt-link></li>
            </ul>
            <div class="text-secondary"><small>&copy; Hak Cipta Codegame</small></div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import { Icon } from '@iconify/vue2';
export default {

  name: 'Footer',

  components: {
    Icon
  },

  data () {
    return {

    }
  }
}
</script>

<style lang="scss" scoped>
  .card{
    &:hover{
      color: #ff5a5e;
    }
  }
</style>