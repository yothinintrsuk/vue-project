<template>
        <div class="app-wrapper container-fluid">
            <NavBar/>
            <parallax>
                <img src="../assets/bg-header.jpg" alt="very cool bg">
            </parallax>
            <BackgroundCover/>
        </div>
</template>

<script>
import NavBar from './navbar'
import BackgroundCover from './background'
import Parallax from 'vue-parallaxy'
export default {
  name: 'home',
  components: {
    NavBar,
    BackgroundCover,
  }
}
</script>

<style lang="scss" scoped>
.app-wrapper{
    padding:0;
    height:100vh;
    background-image:url('../assets/bg-header.jpg');
    background-position: center 0px;
}
</style>
