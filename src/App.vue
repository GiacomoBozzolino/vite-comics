<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components:{
    AppHeader,
    AppMain,
    AppFooter,
  }
  
}
</script>


<template lang="">
  <div  class="container">
    <div>
      <AppHeader/>
    </div>
    <div>
      <AppMain/>
    </div>
    <div>
      <AppFooter/>
    </div>

  </div>
  
    

  
</template>


<style lang="scss" >
@use '../styles/generals.scss' as*




  
</style>