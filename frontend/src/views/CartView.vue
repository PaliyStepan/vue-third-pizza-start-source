<template>
  <div v-if="showYes">yes</div>
  <span v-else>no</span>
</template>

<script>
import { h, ref } from 'vue';

const showYes = ref(true)

export default {
  setup() {
    return () => h('div', [showYes.value ? h('div', 'yes') : h('span', 'no')])
  }
}

</script>

<style scoped>

</style>
