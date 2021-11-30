<template>
  <div class="cds-container">
    <div class="cd" v-for='cd in elements' :key="cd">
        <img :src="cd.poster" :alt="cd.title">
        <h3>{{ cd.title }}</h3>
        <div>{{ cd.author }}</div>
        <div>{{ cd.year }}</div>
    </div>
  </div>
</template>

<script>
import axios from 'axios'
export default {
  name: 'Disk',
  data () {
    return {
      url: 'https://flynn.boolean.careers/exercises/api/array/music',
      elements: null
    }
  },
  mounted: function () {
    axios
      .get(this.url)
      .then(response => {
        (this.elements = response.data.response)
      })
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.DIsk{
    background-color: #2e3a46;
}

.cds-container {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    // padding: 100px 0;
}

.cd {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    flex-direction: column;
    flex-basis: 200px;
    padding: 20px;
    margin: 10px 20px;
    height: 360px;
    background: rgb(46, 58, 70);
    text-align: center;
}

.cd img {
    max-width: 100%;
}

.cd h3 {
    margin: 20px 0;
    color: white;
    font-size: 22px;
    text-transform: uppercase;
}

.cd span.author {
    color: grey;
    font-size: 20px;
}

.cd span.year {
    color: grey;
}
</style>
