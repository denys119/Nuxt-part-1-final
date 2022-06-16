<template>
  <div>
    <h1>
      User page
    </h1>
    <button @click="goBack">
      Go back
    </button>
  </div>
</template>

<script setup lang="ts">
const router = useRouter();
const goBack = () => {
  router.back();
}
</script>