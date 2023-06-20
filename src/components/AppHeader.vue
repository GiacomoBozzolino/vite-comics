<script>
     export default {
        data() {
            return {
                links: [
                    {
                        label : 'CHARACTERS',
                        link: '#',
                        active: false,
                        
                    },
                    {
                        label : 'COMICS',
                        link: '#',
                        active: true,
                        
                    },
                    {
                        label : 'MOVIES',
                        link: '#',
                        active: false,
                        
                    },
                    {
                        label : 'TV',
                        link: '#',
                        active: false,
                        
                    },
                    {
                        label : 'GAMES',
                        link: '#',
                        active: false,
                        
                    },
                    {
                        label : 'COLLECTIBLES',
                        link: '#',
                        active: false,
                        
                    },
                    {
                        label : 'VIDEOS',
                        link: '#',
                        active: false,
                        
                    },
                    {
                        label : 'FANS',
                        link: '#',
                        active: false,
                        
                    },
                    {
                        label : 'NEWS',
                        link: '#',
                        active: false,
                        
                    },
                    {
                        label : 'SHOP',
                        link: '#',
                        active: false,
                        
                    },
                ]
            }
        },
        
    }
</script>

<template lang="">
    <header class="container">
        <div>
            <img src="/assets/dc-logo.png" alt="">
        </div>
        <div>
            <ul>
                <li v-for="(item, index) in links" :class="item.active ? 'active' : ''" :key="index">
                    <a :href="item.link">{{item.label}}</a>
                </li>
            </ul>
        </div>
    </header>
</template>

<style lang="scss" scoped>
header{
   
    display: flex;
    height: 150px;
    padding: 20px;
    justify-content: space-between;
    align-items: center;
    
}

ul{
    display: flex;
    flex-wrap: wrap;
    height: 150px;
    align-items: center;
    li{
        display: flex;
        margin: 0 10px;
        height: 100%;
       align-items: center;
       padding-bottom: 5px;
     
        
    }
}
.container{
    max-width: 1400px;
    margin: 0 auto;
  }

  .active{
    border-bottom: 5px solid #1F81FA;
    padding-bottom: 0;
    
        a{
            color:#1F81FA
        }
  }
</style>