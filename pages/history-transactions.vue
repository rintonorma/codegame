<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-12 col-lg-6 offset-lg-3">
          <div class="card border-0 rounded shadow-sm">
            <div class="card-header border-bottom">
              <div class="d-flex align-items-center gap-2">
                <Icon icon="bx:bx-time" height="24px" style="color: #FF5A5F;"/>
                <h5 class="m-0">History Transaksi</h5>      
              </div>
            </div>
            <div class="card-body">
              <div class="d-grid gap-3">
                <div class="d-flex align-items-center justify-content-between py-3 border-bottom" v-for="i in 10" :key="i">
                  <div class="d-grid gap-2">
                    <div class="fw-bold">1x Mobile Legends, 400 Diamonds + 80 Bonus</div>
                    <div class="text-secondary"><small>30 Sep 2020</small></div>
                  </div>
                  <button class="btn btn-primary rounded">Beli Lagi</button>
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

  name: 'history-transactions',

  layout: 'default',

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