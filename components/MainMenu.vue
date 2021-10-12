<template>
  <div class="position-relative h-100">
    <div class="d-flex align-items-center gap-3 mb-4">
      <div class="avatar ratio ratio-1x1">
        <!-- <img src="/img/"> -->
        H
      </div>
      <div class="d-grid gap-2 text-white">
        <h5 class="m-0">Hunter666@gmail.com</h5>
        <div>Bergabung sejak 30 Sep 2020</div>
      </div>
    </div>
    <ul>
      <li v-for="item in mainmenu" :key="item.id">
        <nuxt-link to="" class="btn rounded p-3 d-flex align-items-center gap-2 text-white" :class="{'active' : item.current}"><Icon :icon="item.icon" height="24px"/><h5 class="m-0">{{ item.text }}</h5></nuxt-link>
      </li>
    </ul>
    <div class="position-absolute bottom-0 w-100 border-top border-primary py-3">
      <nuxt-link to="" class="btn rounded p-3 d-flex align-items-center gap-2 text-white"><Icon icon="bx:bxs-log-out" height="24px"/><h5 class="m-0">Keluar</h5></nuxt-link>
    </div>
  </div>
</template>

<script>
import { Icon } from '@iconify/vue2';
export default {

  name: 'MainMenu',

  components: {
    Icon
  },

  data () {
    return {
      mainmenu: [
        {
          id: 1,
          icon: 'ci:home-fill',
          text: 'Halaman Utama',
          url: '',
          current: true,
        },
        {
          id: 2,
          icon: 'ri:file-history-fill',
          text: 'Histori Transaksi',
          url: '',
          current: false,
        },
      ],
    }
  }
}
</script>

<style lang="css" scoped>
.active{
  background: #FF5A5F;
  color: white;
}
</style>