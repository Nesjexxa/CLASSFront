<template>
  <studentIndex></studentIndex>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import studentIndex from '@/components/studentEnd/studentIndex'

export default defineComponent({
  name: 'Home',
  components: {
    studentIndex
  }
})
</script>
