<template>
  <div id="banner">
    <div id="logo">
      <img src="@/assets/img/logo-spotify.png" alt="">
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#banner {
  height: 80px;
  background-color: #2e3a46;
  display: flex;
}
#logo{
  color: white;
  display: flex;
  align-items: center;
  margin-left: 20px;
}
img{
  height: 50px;
}
</style>
