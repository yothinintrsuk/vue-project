<template>
        <div class="app-wrapper container-fluid">
            <NavBar/>
            <ContentHeader/>
            <Gallery/>
            <!-- <BackgroundCover/> -->
        </div>
</template>

<script>
import NavBar from './navbar'
import BackgroundCover from './background'
import ContentHeader from './contentHeader'
import Gallery from './gallery'
export default {
  name: 'home',
  components: {
    NavBar,
    BackgroundCover,
    ContentHeader,
    Gallery
  }
}
</script>

<style lang="scss" scoped>
.app-wrapper{
    padding:0;
    height:1500px;
    .md-content {
        overflow: auto;
    }
}
</style>
