<script setup>
import { ref, computed } from 'vue'
import store from "../store"

defineProps({
  msg: String,
})
const test = computed(() => store.state.test)
const count = ref(0)
</script>
<template>
{{ test }}
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
