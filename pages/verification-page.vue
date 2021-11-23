<template>
  <section class="container" style="height:100vh">
    <div class="row">
      <div class="col-12 col-lg-6 offset-lg-3">
        <div class="card border-0 rounded shadow-sm">
          <div class="card-body">
            <div class="d-grid gap-3 text-center">
              <Icon icon="bi:check-circle-fill" height="72px" class="m-auto" style="color: #4caf50;"/>
              <h5 class="m-0">Verifikasi Akun Berhasil</h5>   
              <p>Selamat! Akun Anda telah siap digunakan. Masuk ke dashboard Anda sekarang</p>  
              <button class="btn btn-primary btn-lg">Masuk</button> 
              <button class="btn btn-link">Kembali ke Beranda</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import { Icon } from '@iconify/vue2';
export default {

  name: 'verification-page',

  layout: 'pages',

  components: {
    Icon
  },

  data () {
    return {

    }
  }
}
</script>

<style lang="css" scoped>
</style>