<template>
  <div>
    <h1>
      Index page
    </h1>
    <button @click="goToUserPage">
      Go to user page
    </button>
    <nuxt-link to="/user">
      User
    </nuxt-link>
    <nuxt-link to="/user/1?region=England">
      User with id 1
    </nuxt-link>
    <nuxt-link to="/user/name/denis">
      User with name denis
    </nuxt-link>
    <base-component />
  </div>
</template>

<script setup lang="ts">
definePageMeta({
  layout: "default"
})
const router = useRouter();
const goToUserPage = () => {
  router.push({ path: '/user' })
}
</script>