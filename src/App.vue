<script >
// import Componente from './components/Componente';
import TheBigFooter from './components/TheBigFooter.vue';
import TheSmallFooter from './components/TheSmallFooter.vue';
import TheMain from './components/TheMain.vue';
import TheHeader from './components/TheHeader.vue';
import TheNavBar from './components/TheNavBar.vue';


  export default{
    // components:{Componente},
    components:{TheBigFooter,TheSmallFooter,TheMain,TheHeader,TheNavBar},
  }

</script>

<template>
  <!-- <componente></componente> -->


    <TheNavBar></TheNavBar>
    <TheHeader></TheHeader>
    <TheMain></TheMain>
    <TheBigFooter></TheBigFooter>
    <TheSmallFooter></TheSmallFooter>

</template>

<style lang="scss">
@use "./styles/general.scss";

</style>
