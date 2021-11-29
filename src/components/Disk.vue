<template>
  <div>
    <div class="disk-card">
        <img :src="disk.poster" :alt="disk.title">
        <h3>{{ disk.title }}</h3>
        <div>{{ disk.author }}</div>
        <div>{{ disk.year }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Disk',
  data () {
      return {
          disk:{
              'cover':'',
              'title':'',
              'author':'',
              'year':'',
              'type':''

          }
      }
  }
  
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.DIsk{
    background-color: #2e3a46;
}
</style>
