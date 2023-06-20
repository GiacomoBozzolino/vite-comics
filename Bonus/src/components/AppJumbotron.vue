<script>
    export default {
        data() {
            return {
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

.container{
    max-width: 1400px;
    margin: 0 auto;
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
    
</style>