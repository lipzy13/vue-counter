<template>
  <div class="flex items-center justify-center w-20 h-20 bg-white/30 rounded-lg shadow-lg backdrop-blur-md">
            <h1 class="text-3xl font-bold">{{num}}</h1>
  </div>
</template>

<script>
export default {
  props: {
    num: {
      type: Number,
      default: 0,
    },
  }
}
</script>

<style>

</style>