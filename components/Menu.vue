<template>
  <svg
    class="mob-menu"
    width="20"
    height="12"
    viewBox="0 0 75 45"
    xmlns="http://www.w3.org/2000/svg"
    @click="$emit('clicked')"
  >
    <rect x="0" y="0" width="75" height="5"></rect>
    <rect x="0" y="20" width="75" height="5"></rect>
    <rect x="0" y="40" width="75" height="5"></rect>
  </svg>
</template>

<style scoped>
.mob-menu {
  fill: #fff;
}
</style>
