<template>
  <div class="home">
    <studentIndex></studentIndex>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import studentIndex from '@/components/studentEnd/studentIndex.vue'

export default defineComponent({
  name: 'Home',
  components: {
    studentIndex
  }
})
</script>

<style scoped>
home{
}
</style>
