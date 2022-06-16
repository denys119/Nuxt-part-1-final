<template>
  <div>
    <h1>
      User with id parameter {{ route.params.id }}
    </h1>
    <p>
      Region: {{ route.query.region }}
    </p>
  </div>
</template>

<script setup lang="ts">
definePageMeta({
  layout: "default"
})
const route = useRoute();
console.log(route.params.id);
</script>