<template>
<div class="container text-gray-300 px-5 py-24 mx-auto">
  <div class="flex flex-wrap -m-4">
    <project v-for="data in jsonData" :name="data.name" :description="data.desc" :language="data.lang" :url="data.url" :thumbnail="getThumb(data.thumbnail)"/>
  </div>
</div>
</template>

<script>
  import jsonData from "~/assets/projects/projects.json"
  export default {
    name: "Projects",
    data: () => {
      return {
        jsonData: jsonData
      }
    },
    methods: {
      getThumb: function (thumb) {
        return require(`~/assets/projects/thumbnails/${thumb}`);
      }
    }
  }
</script>
