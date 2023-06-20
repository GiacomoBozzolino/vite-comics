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
                        img:'../assets/buy-comics-subscription.png',
                    },
                    {
                        label: 'COMIC SHOP LOCATOR',
                        img:'../assets/buy-comics-shop-locator.png',
                    },
                    {
                        label: 'DC POWER VISA',
                        img :'../assets/buy-dc-power-visa.svg',
                    },
                ]
            }
        },
        
    }
</script>

<template lang="">
    <div class="container">
        <div class="content">
            <div> --Content goes here-- </div> 
            
        </div>
        <div class="blue-content">
            <ul>
                <li v-for="(item, index) in menu" :key="index">
                    <img :src="item.img" alt="">
                    <div>{{item.label}}</div>
                </li>
                <img src="../assets/buy-comics-digital-comics.png" alt="">
                
            </ul>
        </div>

    </div>
</template>


<style lang="scss" scoped>
.content{
    height: 150px;
    background-color: black;
    color: white;
    display: flex;
    align-items: center;
        div{
            font-size: 40px;
            padding: 0 20px; 
        }
}


.blue-content{
    height: 200px;
    background-color:#1F81FA ;
        ul{
            display: flex;
            padding: 0 20px;
            justify-content: space-between;

            
        }

}
    
</style>