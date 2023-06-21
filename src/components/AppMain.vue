<script>
import comics from '../data/dc-comics.js';
import AppComics from './AppComics.vue';

    export default {
        components: {
            comics,
            AppComics
        },


        data() {
            return {
                NewComics: comics,


                menu: [
                    {
                        label: 'DIGITAL COMICS',
                        img:'../assets/buy-comics-digital-comics.png',
                    },
                    {
                        label: 'DC MERCHANDISE',
                        img:'../assets/buy-comics-merchandise.png',
                    },
                    {
                        label: 'SUBSCRIPTION',
                        img:'../assets/buy-comics-subscriptions.png',
                    },
                    {
                        label: 'COMIC SHOP LOCATOR',
                        img:'../assets/buy-comics-shop-locator.png',
                    },
                    {
                        label : 'DC POWER VISA',
                        img :'../assets/buy-dc-power-visa.svg',
                    },
                ]
            }
        },
        
    }
</script>

<template lang="">
    <div >
        <img id="jumbo" src="/assets/jumbotron.jpg" >
    </div>
    <div class="black">
        <div class="container content">
            <div id="series">CURRENT SERIES</div>
            <div class="flex flex-wrap">
                <AppComics v-for="(comics, index) in NewComics" :key="index" :recentComics='comics'  /> 
            </div>
            
        </div>
    </div>
    <div class="blue">
        <div class="container blue-content">
            <ul>
                <li v-for="(item, index) in menu" :key="index">
                    <a href="#">
                        <img :src="item.img" alt="">
                        <div>{{item.label}}</div>
                    </a>
                </li>   
            </ul>
        </div>
    </div>
   
</template>


<style lang="scss" scoped>
.blue{
    background-color:#1F81FA ;
}
.black{
    background-color: black;
}

.content{
    position: relative;
    // height: 150px;
    color: white;
    display: flex;
    align-items: center;
        // div{
        //     font-size: 40px;
        //     padding: 0 20px; 
        // }
}


.blue-content{
    height: 200px;
    
    display: flex;
    justify-content: center;
        ul{
            display: flex;
            padding: 0 80px;
           justify-content: space-around;
           flex-wrap: wrap;

           li{
               display: flex;
               padding: 0 20px;
               a{
                    display: flex;
                    color: white;
                    align-items: center;
                       img{
                           width: 50px;
                           margin: 0 10px;  
                       }  
                }

           };
        }

}

#jumbo{
    display: flex;
    height: 45vh;
    width: 100%;
    object-fit: cover;
    object-position: top center;
}

#series{
    position: absolute;
    color: white;
    font-size: 20px;
    background-color: #1F81FA;
    padding: 10px 20px;
    font-weight: bold;
    top: -25px;


}
</style>