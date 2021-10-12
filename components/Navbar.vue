<template>
  <div class="bg-white shadow sticky-top">
    <div class="container">
      <div class="d-flex align-items-center justify-content-between">
        <div class="d-flex align-items-center">
          <a href="" class="text-danger" data-bs-toggle="offcanvas" href="#offcanvas1" role="button" aria-controls="offcanvas1"><Icon icon="ci:menu-alt-03" height="24px"/></a>
          <nuxt-link to="/" class="p-3"><img src="~/static/img/logo.svg"></nuxt-link>
        </div>
        <div class="input-group btn-search bg-white border rounded-pill d-none d-lg-flex">
          <button class="btn bg-transparent text-danger" type="button">
            <Icon icon="bx:bx-search" height="24px"/>
          </button>
          <input type="search" class="form-control bg-transparent border-0" placeholder="Pencarian game ataupun voucher" ref="control" @keyup.enter="find">
        </div>
        <div class="d-inline-block d-lg-none">
          <button class="bg-transparent border-0 text-danger" type="button" data-bs-toggle="collapse" data-bs-target="#collapseExample" aria-expanded="false" aria-controls="collapseExample">
            <Icon icon="bx:bx-search" height="24px"/>
          </button>
        </div>
      </div>
      <div class="collapse pb-3" id="collapseExample">
        <input type="search" class="form-control bg-transparent border rounded-pill" placeholder="Pencarian game ataupun voucher" ref="control" @keyup.enter="find">
      </div>
    </div>
  </div>
</template>

<script>
import { Icon } from '@iconify/vue2';
export default {

  name: 'Navbar',

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