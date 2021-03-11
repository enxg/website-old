<template>
  <div>
    <div class="border-2 border-gray-800 px-5 py-3 text-gray-200  rounded">
      <h1 class="text-xl align-middle"><i class="fas fa-graduation-cap mr-2"></i>Skills</h1>
      <div v-for="skill in skills">
        <aboutSkill v-bind:name="skill.name" v-bind:value="skill.value" v-bind:icon="skill.icon" />
      </div>
    </div>
  </div>
</template>

<script>
import skills from "~/assets/skills.json";
skills.sort((a,b) => {
  return b.value - a.value
})

export default {
  name: "aboutSkills",
  data: () => {
    return({
      skills: skills
    })
  }
}
</script>
