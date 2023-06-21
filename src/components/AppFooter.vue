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
        <div class="container flex">
            <div class="upper-footer">
                <div>
                    <h3>DC COMICS</h3>
                    <ul>
                        <li v-for="(item, index) in comics" :key="index">
                            <a :href="item.link">{{item.label}}</a>
                        </li>
                    </ul>
    
                    
                        <h3>SHOP</h3>
                    <ul>
                        <li>
                            <a href="#">Shop DC</a>
                        </li>
                        <li>
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
            </div>
            <div class="logo">
                <!-- <img src="assets/dc-logo-bg.png" alt=""> -->
            </div> 
        </div>
        <div class="lower-footer  ">
            <div class="container">
                <div class="row">
                    <div class="lower-content flex">
                        <div>
                            <button>SIGN-UP NOW!</button>
                        </div>
                        <div>
                            <h3>FOLLOW US</h3>
                            <ul class="flex">
                                <li>
                                    <a href="#">
                                        <img src="assets/footer-facebook.png" alt="">
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        <img src="assets/footer-twitter.png" alt="">
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        <img src="assets/footer-youtube.png" alt="">
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        <img src="assets/footer-pinterest.png" alt="">
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        <img src="assets/footer-periscope.png" alt="">
                                    </a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </footer>

</template>

<style lang="scss" scoped>

footer{
    background-image: url(public/assets/footer-bg.jpg);
    background-size: cover;
}
.container{
    max-width: 1400px;
    margin: 0 auto;
  }

.upper-footer{
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
    font-size: 17px;
    padding: 10px 0;
}

.container.flex{
    justify-content: space-between;
}
.logo{
    background-image: url(public/assets/dc-logo-bg.png);
    max-height:40%;
    width: 40%;
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover
}
.lower-footer{
    background-color: #303030;
    height: 100px;
        .container{
            height: 100%;

            button{
                padding: 20px;
                background-color: transparent;
                border: 2px solid #1F81FA;
                color: white;
                font-size: 17px;
                font-weight: bold;
                cursor: pointer;

            }
        }
    

}


.lower-content{
    height: 100%;
    width: 100%;
    justify-content: space-between;
    align-items: center;
     div{
            display: flex;
            h3{
                color: #1F81FA;
                margin-right: 20px;
                font-size: 22px;
            }
            ul{
                li{
                    padding: 0 10px;
                }
            }

        }
}
    .row{
        height: 100%;
        padding: 0 20px;
        
    }
</style>