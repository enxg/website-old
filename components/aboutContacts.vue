<template>
  <div>
    <div class="border-2 border-gray-800 px-5 py-3 text-gray-200 rounded">
      <h1 class="text-xl align-middle"><i class="fas fa-comment mr-2"></i>Contact</h1>
      <div v-for="contact in contacts">
        <aboutContact v-bind:icon="contact.icon" v-bind:name="contact.name" v-bind:value="contact.value" />
      </div>
    </div>
  </div>
</template>

<script>
import contacts from "~/assets/contacts.json";

export default {
  name: "aboutContacts",
  data: () => {
    return({
      contacts: contacts
    })
  }
}
</script>
