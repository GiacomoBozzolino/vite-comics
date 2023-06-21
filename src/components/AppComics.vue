<script>

    export default {
        props:{
            recentComics: Object

        }
        
    }
</script>

<template lang="">
   
        <div class="card">
            <img :src="recentComics.thumb" alt="">
            <h5 v-text="recentComics.series"></h5>

        </div>
        
    

</template>


<style lang="scss" scoped>
.card{
    padding-top: 40px;
    width: calc(100%/6 - 40px);
    margin: 20px;
    h5{
        text-align: left
    }
    img{
        width: 190px;
        height: 250px;
        padding-bottom: 10px;
    }
}

</style>