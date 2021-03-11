<template>
  <div class="my-3">
    <h1 class="mb-1 align-middle"><i :class="icon" class="mx-0.5"></i> {{ name }}</h1>
    <progressBar v-bind:value="value"/>
  </div>
</template>

<script>
export default {
  name: "aboutSkill",
  props: ["name", "value", "icon"]
};
</script>

<style scoped>

</style>
