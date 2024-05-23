<script>
export default {
  data() {
    return {
      linkList: [
        'CHARACTERS',
        'COMICS',
        'MOVIES',
        'TV',
        'GAMES',
        'COLLECTIBLES',
        'VIDEOS',
        'FANS',
        'NEWS',
        'SHOP'
      ]
    }
  }
}

</script>

<template>
  <div class="contenitore">

    <div class="row" style="height: 100%;">

      <div class="col-4 align-content-center">
        <div style="width: 10%;">
          <img src="../../img/dc-logo.png" alt="" style="width: 100%;">
        </div>
      </div>

      <div class="col-8 align-content-center">
        <div class="d-flex">
          <div v-for="link in linkList" class="single-link">
            {{ link }}
          </div>
        </div>
      </div>

    </div>

  </div>
</template>

<style scoped>
.single-link {
  text-align: center;
  font-size: 0.7rem;
  margin: 0 1rem;
}
</style>
