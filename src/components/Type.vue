<template>
    <div id="container">
        <div>
            <div>
                <div id="genere">SELEZIONA GENERE:</div>
                <select>
                    <option value="all">All</option>
                    <option value="rock">Rock</option>
                    <option value="pop">Pop</option>
                    <option value="jazz">Jazz</option>
                    <option value="metal">Metal</option>
                </select>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Type'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    #container {
        text-align: center;
        background-color: #1e2d3b;
    }
    select{
        height: 50px;
        font-size: 20px;
    }
    #genere{
        padding: 20px;
        color: white;
    }

</style>
