<template>
  <div>
    <h1>
      User with name parameter {{ route.params.name }}
    </h1>
  </div>
</template>

<script setup lang="ts">
definePageMeta({
  layout: "admin"
})
const route = useRoute();
console.log(route.params.name);
</script>