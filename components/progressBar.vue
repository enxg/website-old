<template>
  <div class="h-3 relative max-w-xl rounded-full overflow-hidden">
    <div class="w-full h-full bg-gray-800 absolute"></div>
    <div class="h-full bg-green-500 absolute" :style="{width: value + '%'}"></div>
  </div>
</template>

<script>
export default {
  name: "progressBar",
  props: ["value"]
}
</script>

<style scoped>

</style>
