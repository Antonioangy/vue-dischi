<template>
  <main>
    <Disk/>
  </main>
</template>

<script>
import Disk from '@/components/Disk.vue'
export default {
  name: 'Main',
  components: {
    Disk
  }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
Main{
  height: 100vh;
  background-color: #1e2d3b;
}

</style>
