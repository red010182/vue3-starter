<script setup lang="ts">
const { name } = defineProps({
  name: String,
})
const router = useRouter()
</script>

<template lang="pug">
p Hello, {{ name }}
button.btn.mt-4(@click='router.back()') Back
</template>
