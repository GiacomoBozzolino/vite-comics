<script>
    export default {
        data() {
            return {
                // primo array
                comics : [
                    {
                        label:'Characters',
                        link: '#',
                    },
                    {
                        label:'Comics',
                        link: '#',
                    },
                    {
                        label:'Movies',
                        link: '#',
                    },
                    {
                        label:'TV',
                        link: '#',
                    },
                    {
                        label:'Games',
                        link: '#',
                    },
                    {
                        label:'Videos',
                        link: '#',
                    },
                    {
                        label:'News',
                        link: '#',
                    },
                ],
                    // secondo array
                info : [
                    {
                        label:'Terms Of Use',
                        link: '#',
                    },
                    {
                        label:'Privacy policy(New)',
                        link: '#',
                    },
                    {
                        label:'Ad Choices',
                        link: '#',
                    },
                    {
                        label:'Advertising',
                        link: '#',
                    },
                    {
                        label:'Jobs',
                        link: '#',
                    },
                    {
                        label:'Subscription',
                        link: '#',
                    },
                    {
                        label:'Talent Workshop',
                        link: '#',
                    },
                    {
                        label:'CPSC Certificates',
                        link: '#',
                    },
                    {
                        label:'Ratings',
                        link: '#',
                    },
                    {
                        label:'Shop Help',
                        link: '#',
                    },
                    {
                        label:'Contact Us',
                        link: '#',
                    },
                ],
                    // terzo array
                sites : [
                    {
                        label:'DC ',
                        link: '#',
                    },
                    {
                        label:'MAD Magazine',
                        link: '#',
                    },
                    {
                        label:'DC Kids',
                        link: '#',
                    },
                    {
                        label:'DC Universe',
                        link: '#',
                    },
                    {
                        label:'DC power Visa',
                        link: '#',
                    },
                ]

                
            }
        },
        
    }
</script>

<template lang="">
    <footer>
        <div class="upper-footer container">
            <div>
                <h3>DC COMICS</h3>
                <ul>
                    <li v-for="(item, index) in comics" :key="index">
                    <a :href="item.link">{{item.label}}</a>
                </li>
                </ul>

                
                    <h3>SHOP</h3>
                <ul>
                    <li >
                        <a href="#">Shop DC</a>
                    </li>
                    <li >
                        <a href="#">Shop DC Collectibles</a>
                    </li>
                </ul>
            </div>

            <div>
                <h3>DC </h3>
                <ul>
                    <li v-for="(item, index) in info" :key="index">
                    <a :href="item.link">{{item.label}}</a>
                </li>
                </ul>
            </div>
            <div>
                <h3>SITES</h3>
                <ul>
                    <li v-for="(item, index) in sites" :key="index">
                    <a :href="item.link">{{item.label}}</a>
                </li>
                </ul>
            </div>
            <div class="logo">
                <img src="assets/dc-logo-bg.png" alt="">
            </div> 
        </div>
        <div class="lower-footer ">
            <div class="container">

            </div>
        </div>


    </footer>

</template>

<style lang="scss" scoped>

footer{
    background-image: url(public/assets/footer-bg.jpg);
}
.container{
    max-width: 1400px;
    margin: 0 auto;
  }

.upper-footer{
    position: relative;
    
    height: 400px;
    background-size: cover;
    display: flex;
        div{
            padding: 20px;
            color: white;
                ul{
                    li{
                        padding: 2px 0;
                        a{
                            color: #959595;
                        }
                    }
                    
                }
        }
}

h3{
    font-size: 20px;
    padding: 10px 0;
}
.logo{
    position: absolute;
    top: -100px;
    right: 0;
    
}
.lower-footer{
    background-color: #303030;
    height: 100px;
    z-index: 100;
    
}
    
</style>