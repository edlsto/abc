<template>
  <div class="ctn">
    hi
  </div>
</template>

<script>
export default {
  async asyncData ({ $http }) {
    const mountains = await $http.$get('https://f.v1.n0.cdn.getcloudapp.com/items/3e1W2F0W1s2U2d3R2Z46/content.json')
    console.log(mountains)
    return { mountains }
  }
}
</script>

<style scoped>

.ctn {
  height: 100vh;
  background: green;
  position: absolute;
  min-height: 100vh;
  width: 100vw;
  top: 0;
  z-index: -1;
  padding-top: 10rem;
  font-size: 3rem;
  box-sizing: border-box;
  /* background-image: url('/shot.png') */
}

</style>
