<template>
  <header class="text-gray-400 bg-gray-900 body-font border-b-2 border-gray-800">
    <div class="container mx-auto flex flex-wrap p-5 flex-col md:flex-row items-center">
      <a class="flex title-font font-medium items-center text-white mb-4 md:mb-0">
        <span class="text-xl">Enes Genç</span>
      </a>
      <button v-on:click="isOpen = !isOpen" class="py-1 px-3 my-2 border-2 border-green-500 text-green-500 md:hidden sm:block rounded hover:text-white hover:bg-green-500 duration-200">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
        </svg>
      </button>
      <nav :class="isOpen ? 'flex' : 'hidden'" class="md:ml-auto space-y-2 md:space-y-0 md:flex md:flex-row flex-col items-center overflow-hidden text-base justify-center">
        <NuxtLink to="/" class="mx-2.5 hover:text-white" exact-active-class="text-white">Home</NuxtLink>
        <NuxtLink to="/projects" class="mx-2.5 hover:text-white" exact-active-class="text-white">My Projects</NuxtLink>
        <NuxtLink to="/about" class="mx-2.5 hover:text-white" exact-active-class="text-white">About Me</NuxtLink>
        <NuxtLink to="/about" class="inline-flex items-center duration-200 justify-center border-2 py-1 px-3 focus:outline-none hover:bg-green-500 hover:text-white text-green-500 border-green-500 rounded text-base ml-2.5 mt-4 md:mt-0" exact-active-class="text-white">Contact
          <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4 ml-1 text-sm" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
          </svg>
        </NuxtLink>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "NavBar",
  data: () => {
    return {
      isOpen: false
    }
  },
  props: ["sas"]
}
</script>

<style scoped>

</style>
