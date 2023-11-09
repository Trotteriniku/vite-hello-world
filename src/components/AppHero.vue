<template>
    <div class="containerHero">
        <div v-for="photoindex in 8" class="card pad z">
            <img  :src="'/public/backa'+photoindex+'.jpg'" alt="fotine">
        </div>
    </div>
</template>

<script>
    export default {
        name : 'AppHero',
        
    }
</script>

<style lang="css" scoped>
    .containerHero{
        margin: 50px auto;
        display: flex;
        flex-wrap: wrap;
        width: 60%;
        height: 80%;
        border: 1px solid black;
        padding: 10px;
        background-color:#53b1b1;
        border: 10px groove #53b1b1;
    }
    .card{
        margin: 10px;
        width: calc(100% / 4 - 20px);
        border: 4px outset #f69000;
        border-radius: 5%;
        overflow: hidden;
    }

    img{
        width: 100%;
        height: 100%;
        display: block;

    }
</style>