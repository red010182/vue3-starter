<script setup lang="ts">
const name = ref('someone')
</script>

<template lang="pug">
input.p2.border(v-model='name')
p Hello, {{ name }}
q-btn hi
</template>
