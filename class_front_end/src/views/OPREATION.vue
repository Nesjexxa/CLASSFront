<template>
<div>
<IMView></IMView>
  <operationView></operationView>
</div>
</template>

<script>
import IMView from '@/components/operation/IMView.vue'
import operationView from '@/components/operation/operationView.vue'
export default {
  name: 'OPREATION',
  components: {
    IMView,
    operationView
  }
}
</script>

<style scoped>

</style>
