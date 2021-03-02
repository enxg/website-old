<template>
  <section class="text-gray-300 bg-gray-900 body-font">
    <div class="container mx-auto flex px-5 py-12 flex-col justify-center items-center text-center">
      <img src="~/assets/pfp.png" class="rounded-full w-auto h-60 object-cover mb-10" alt="Hi 👋">
      <h1 class="text-3xl">Hi 👋</h1>
      <p class="text-xl mt-2 mb-5">I am <strong>Enes Genç</strong>. I work as front-end, back-end, mobile developer.</p>
      <NuxtLink to="contact" class="border-2 flex align-middle items-center justify-center rounded text-green-500 border-green-500 px-3 py-1 hover:bg-green-500 hover:text-white duration-200"><span>Contact</span>
        <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4 ml-1 text-sm" fill="none" viewBox="0 0 24 24" stroke="currentColor">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
      </svg>
      </NuxtLink>
    </div>
  </section>
</template>

<script>
export default {
  name: "indexHero"
};
</script>

<style scoped>

</style>
