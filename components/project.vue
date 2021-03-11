<template>
  <div class="p-4 md:w-1/3">
    <div class="h-full border-2 border-gray-800 rounded-lg overflow-hidden">
      <img class="lg:h-48 md:h-36 w-full object-cover object-center" :src="thumbnail" alt="blog">
      <div class="p-6">
        <h2 class="tracking-widest text-xs title-font font-medium text-gray-500 mb-1 uppercase">{{ language }}</h2>
        <h1 class="title-font text-lg font-medium text-white mb-3">{{ name }}</h1>
        <p class="leading-relaxed h-full mb-3">{{ description }}</p>
        <div class="flex items-center flex-wrap w-auto">
          <a :href="url" class="text-green-500 px-3 py-1 border-green-500 border-2 text-center justify-center rounded min-w-full inline-flex items-center align-middle md:mb-2 lg:mb-0 hover:bg-green-500 hover:text-white duration-200">Learn More
            <svg class="w-5 h-5 ml-1" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round">
              <path d="M5 12h14"></path>
              <path d="M12 5l7 7-7 7"></path>
            </svg>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "project",
  props: ["name", "description", "language", "thumbnail", "url"]
}
</script>

