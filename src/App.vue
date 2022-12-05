<script >
// import Componente from './components/Componente';
import TheBigFooter from './components/TheBigFooter.vue';
import TheSmallFooter from './components/TheSmallFooter.vue';
import TheMain from './components/TheMain.vue';
import TheHeader from './components/TheHeader.vue';
import TheNavBar from './components/TheNavBar.vue';
import TheImage from './components/TheImage.vue';



  export default{
    // components:{Componente},
    components:{TheBigFooter,TheSmallFooter,TheMain,TheHeader,TheNavBar,TheImage},
  }

</script>

<template>
  <!-- <componente></componente> -->


    <TheNavBar></TheNavBar>
    <TheImage></TheImage>
    <TheHeader></TheHeader>
    <TheMain></TheMain>
    <TheBigFooter></TheBigFooter>
    <TheSmallFooter></TheSmallFooter>
    

</template>

<style lang="scss">
@use "./styles/general.scss";

</style>
