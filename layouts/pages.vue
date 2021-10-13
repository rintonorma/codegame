<template>
  <div>
    <div class="bg-white shadow sticky-top">
      <div class="container">
        <div class="d-flex align-items-center justify-content-between">
          <div class="d-flex align-items-center">
            <nuxt-link to="/" class="py-3"><img src="~/static/img/logo.svg"></nuxt-link>
          </div>
        </div>
      </div>
    </div>
    <div class="bg-gray">
      <Nuxt />
    </div>
  </div>
</template>

<script>
export default {

  name: 'pages',

  data () {
    return {

    }
  }
}
</script>

<style lang="css" scoped>
</style>