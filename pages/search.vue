<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-12 col-lg-6 offset-lg-3">
          <div class="card border-0 rounded shadow-sm">
            <div class="card-header border-bottom">
              <div class="d-flex align-items-center gap-2">
                <h5 class="m-0">Hasil Pencarian</h5>      
              </div>
            </div>
            <div class="card-body">
              <div class="d-grid gap-3">
                <div class="input-group btn-search bg-white border rounded-pill d-none d-lg-flex">
                  <button class="btn bg-transparent text-danger" type="button">
                    <Icon icon="bx:bx-search" height="24px"/>
                  </button>
                  <input type="search" class="form-control bg-transparent border-0" placeholder="Pencarian game ataupun voucher" ref="control" @keyup.enter="find">
                </div>
                <ul class="nav nav-pills gap-2 overflow-auto" id="pills-tab" role="tablist">
                  <li class="nav-item flex-shrink-0" role="presentation">
                    <button class="nav-link active rounded-pill" id="pills-1-tab" data-bs-toggle="pill" data-bs-target="#pills-1" type="button" role="tab" aria-controls="pills-1" aria-selected="true">Semua</button>
                  </li>
                  <li class="nav-item flex-shrink-0" role="presentation">
                    <button class="nav-link rounded-pill" id="pills-2-tab" data-bs-toggle="pill" data-bs-target="#pills-2" type="button" role="tab" aria-controls="pills-2" aria-selected="false">Game Baru</button>
                  </li>
                  <li class="nav-item flex-shrink-0" role="presentation">
                    <button class="nav-link rounded-pill" id="pills-3-tab" data-bs-toggle="pill" data-bs-target="#pills-3" type="button" role="tab" aria-controls="pills-3" aria-selected="false">Voucher</button>
                  </li>
                  <li class="nav-item flex-shrink-0" role="presentation">
                    <button class="nav-link rounded-pill" id="pills-4-tab" data-bs-toggle="pill" data-bs-target="#pills-4" type="button" role="tab" aria-controls="pills-4" aria-selected="false">Video Live</button>
                  </li>
                </ul>
                <div class="games-slider row g-3">
                  <div class="col-4 col-lg-3" v-for="item in games" :key="item.id">
                    <nuxt-link to="/single-product" class="card rounded border-0">
                      <div class="">
                        <div class="ratio ratio-1x1 mb-2">
                          <img :src="item.src" :alt="item.title" class="object-cover rounded">
                        </div>
                        <div class="d-grid gap-1 text-center">
                          <small class="text-secondary">{{ item.publisher }}</small>
                          <div class="card-title text-dark fw-bold mb-0">{{ item.title }}</div>
                        </div>
                      </div>
                    </nuxt-link>
                  </div>
                </div>
                <nav aria-label="...">
                  <ul class="pagination m-0 justify-content-center">
                    <li class="page-item disabled">
                      <span class="page-link">Kembali</span>
                    </li>
                    <li class="page-item"><a class="page-link" href="#">1</a></li>
                    <li class="page-item active" aria-current="page">
                      <span class="page-link">2</span>
                    </li>
                    <li class="page-item"><a class="page-link" href="#">3</a></li>
                    <li class="page-item">
                      <a class="page-link" href="#">Selanjutnya</a>
                    </li>
                  </ul>
                </nav>
              </div>
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

  name: 'search',

  components: {
    Icon
  },

  data () {
    return {
      games: [
        {
          id: 1,
          src: '/img/games/PUBG-Battlegrounds.-Foto-Charlie-INTEL.jpg',
          title: 'PUBG Mobiles',
          publisher: 'Tencent Games',
        },
        {
          id: 2,
          src: '/img/games/4205651984.jpeg',
          title: 'League of Legends',
          publisher: 'Riot Games',
        },
        {
          id: 3,
          src: '/img/games/043189000_1524529114-maxresdefault.jpeg',
          title: 'Mobile Legends: Bang Bang',
          publisher: 'Moontons',
        },
        {
          id: 4,
          src: '/img/games/images-12-696x392.jpeg',
          title: 'Call of Duty: Mobile',
          publisher: 'Activision',
        },
        {
          id: 5,
          src: '/img/games/Garena-Free-Fire.jpeg',
          title: 'Free Fire',
          publisher: 'Garena',
        },
        {
          id: 6,
          src: '/img/games/1725796951.jpeg',
          title: 'Sausage Man',
          publisher: 'XD Entertainment Pte Ltd',
        },
        {
          id: 7,
          src: '/img/games/Spesifikasi-Game-Valorant.jpeg',
          title: 'Valorant',
          publisher: 'Riot Games',
        },
        {
          id: 8,
          src: '/img/games/unnamed.png',
          title: 'Higgs Domino',
          publisher: 'Poker City',
        },
        {
          id: 9,
          src: '/img/games/ragx-nextgen-cbt-news-id-2.jpeg',
          title: 'Ragnarok X: Next Generation',
          publisher: 'Nuverse',
        },
        {
          id: 10,
          src: '/img/games/thumb_ff94b-hago-logo-jpg_adaptiveResize_300_300.jpeg',
          title: 'Hago',
          publisher: 'Hago Games',
        },
        {
          id: 11,
          src: '/img/games/69437-genshin-impact-mihoyo.jpeg',
          title: 'Genshin Impact',
          publisher: 'miHoYo',
        },
        {
          id: 12,
          src: '/img/games/unnamed (1).png',
          title: 'Tinder',
          publisher: 'Tinder',
        },
      ],
    }
  }
}
</script>

<style lang="scss" scoped>
.nav-link{
  color: #2b2d41;
  background-color: white;
  border: 1px solid #ddd!important;
  padding-left: 30px;
  padding-right: 30px;
}
.nav-pills {
  .nav-link.active {
    color: #fff;
    background-color: #ff5a5e;
    border: 1px solid #ff5a5e!important;
  }
}
@media only screen and (max-width: 767px){
  .games-slider{
    margin-left: -15px;
    margin-right: -15px;

    a{

      small{
        font-size: 11px;
      }

      .card-title{
        font-size: 14px;
      }
    }
  }
}
</style>





