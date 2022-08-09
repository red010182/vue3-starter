<script setup lang="ts">
const router = useRouter()
const name = ref('')
const disabled = computed(() => name.value.length === 0)
const greetingAction = () => router.push(`/hi/${name.value}`)
</script>

<template lang="pug">
input.p2.border(v-model='name')
.h-10
  p(v-if='name') Hello, {{ name }}
button.btn(@click='greetingAction', :disabled='disabled') Say Hello
Footer.mt-30
</template>
