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
        <button class="btn btn-primary btn-lg w-100 text-white rounded" type="button">Masuk</button>
      </div>
      <div class="text-white mb-3">Belum punya Akun? <nuxt-link to="" class="btn-link text-primary">Buat Akun</nuxt-link></div>
      <div class="divider-line mb-3">Masuk akun dengan</div>
      <div class="mb-3">
        <div class="position-relative">
          <Icon icon="flat-color-icons:google" height="24px" class="position-absolute top-0 start-0 mx-3 h-100"/>
          <button class="btn btn-light btn-lg w-100 text-dark rounded" type="button">Google</button>
        </div>
      </div>
      <div class="mb-3">
        <div class="position-relative">
          <Icon icon="akar-icons:facebook-fill" height="24px" class="position-absolute top-0 start-0 mx-3 h-100" style="color: #3b5998;"/>
          <button class="btn btn-light btn-lg w-100 text-dark rounded" type="button">Facebook</button>
        </div>
      </div>
    </form>
  </div>
</template>

<script>
export default {

  name: 'Login',

  data () {
    return {

    }
  }
}
</script>

<style lang="css" scoped>
</style>