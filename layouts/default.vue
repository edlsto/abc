<template>
  <div :class="$style.ctn">
    <div :class="$style.header">My header</div>
    <Nuxt />
  </div>
</template>

<style module>

.ctn {
  height: 100vh;
  /* background: green; */
}

.header {
    position: absolute;
    width: 100%;
    border: 1px solid red;
    box-sizing: border-box;
    height: 10rem;
}

</style>
