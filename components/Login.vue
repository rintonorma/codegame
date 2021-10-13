<template>
  <div>
    <h4 class="text-white mb-4">Masuk akun</h4>
    <form>
      <div class="mb-3">
        <label for="emailInput" class="form-label text-white">Email</label>
        <input type="email" class="form-control form-control-lg rounded" id="emailInput" placeholder="Masukkan alamat Email">
      </div>
      <div class="mb-3">
        <label for="passwordInput" class="form-label text-white">Kata Sandi</label>
        <div class="position-relative">
          <input type="password" class="form-control form-control-lg rounded" id="passwordInput" placeholder="Masukkan kata sandi">
          <button class="btn bg-transparent h-100 text-secondary position-absolute top-0 end-0" type="button">
            <Icon icon="carbon:view-filled" height="24px"/>
          </button>
        </div>
      </div>
      <div class="text-white mb-3">Lupa Kata Sandi? <nuxt-link to="" class="btn-link text-primary">Ubah Sandi</nuxt-link></div>
      <div class="mb-3">
        <button class="btn btn-primary btn-lg w-100 text-white rounded" type="button" @click="successLogin">Masuk</button>
      </div>
      <div class="text-white mb-3">Belum punya Akun? <button class="btn-link bg-transparent border-0 text-primary" @click="changeState">Buat Akun</button></div>
      <div class="divider-line mb-3">Masuk akun dengan</div>
      <div class="mb-3">
        <div class="position-relative">
          <button class="btn btn-light btn-lg w-100 text-dark rounded" type="button">
            <Icon icon="flat-color-icons:google" height="24px" class="position-absolute top-0 start-0 mx-3 h-100"/>Google
          </button>
        </div>
      </div>
      <div class="mb-3">
        <div class="position-relative">
          <button class="btn btn-light btn-lg w-100 text-dark rounded" type="button">
          <Icon icon="akar-icons:facebook-fill" height="24px" class="position-absolute top-0 start-0 mx-3 h-100" style="color: #3b5998;"/>Facebook</button>
        </div>
      </div>
    </form>
  </div>
</template>

<script>
import { Icon } from '@iconify/vue2';
export default {

  name: 'Login',

  components: {
    Icon
  },

  data () {
    return {
      
    }
  },
  methods: {
    changeState() {
      this.$emit('changeState', 'register')     
    },
    successLogin() {
      this.$emit('changeState', 'loggedin')
    }
  }
}
</script>

<style lang="css" scoped>
</style>