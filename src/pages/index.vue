<script setup lang="ts">
const name = ref('someone')
const router = useRouter()
</script>

<template lang="pug">
input.p2.border(v-model='name')
p Hello, {{ name }}
</template>
