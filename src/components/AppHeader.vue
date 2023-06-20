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
                        active: false,
                        
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
    <header>
        <div>
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <div>
            <ul>
                <li v-for="(item, index) in links" :key="index">
                    <a :href="item.link">{{item.label}}</a>

                </li>
            </ul>
        </div>
    </header>
</template>

<style lang="scss" scoped>
header{
    max-width: 100vw;
    display: flex;
    height: 150px;
    padding: 20px;
    justify-content: space-between;
    align-items: center;
    
}

ul{
    display: flex;
    flex-wrap: wrap;
    li{
        padding: 0 10px;
    }
}
    
</style>