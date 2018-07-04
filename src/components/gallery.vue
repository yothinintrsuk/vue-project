<template>
    <div class="gallery-cover container-fluid">
        <div class="row">
            <div class="img-cover col-sm-12 col-md-4 col-lg-4">
                <div class="img-box" >
                    <img src="https://demo.themetorium.net/html/sepia/assets/img/gallery/gallery-single/grid/big/gallery-single-big-1.jpg" alt="">
                </div>
                <div v-on:click="say('hi')" class="bg-img-box">
                    <div>
                        <span>The Old Man Dreams</span><br/>
                        <span>Outdoor</span>
                    </div>
                </div>
            </div>
            <div class="img-cover col-sm-12 col-md-4 col-lg-4">
                <div class="img-box">
                    <img src="https://demo.themetorium.net/html/sepia/assets/img/gallery/gallery-single/grid/big/gallery-single-big-1.jpg" alt="">
                </div>
            </div>
            <div class="img-cover col-sm-12 col-md-4 col-lg-4">
                <div class="img-box">
                    <img src="https://demo.themetorium.net/html/sepia/assets/img/gallery/gallery-single/grid/big/gallery-single-big-1.jpg" alt="">
                </div>
            </div>
             <div class="img-cover col-sm-12 col-md-4 col-lg-4">
                <div class="img-box">
                    <img src="https://demo.themetorium.net/html/sepia/assets/img/gallery/gallery-single/grid/big/gallery-single-big-1.jpg" alt="">
                </div>
            </div>
            <div class="img-cover col-sm-12 col-md-4 col-lg-4">
                <div class="img-box">
                    <img src="https://demo.themetorium.net/html/sepia/assets/img/gallery/gallery-single/grid/big/gallery-single-big-1.jpg" alt="">
                </div>
            </div>
            <div class="img-cover col-sm-12 col-md-4 col-lg-4">
                <div class="img-box">
                    <img src="https://demo.themetorium.net/html/sepia/assets/img/gallery/gallery-single/grid/big/gallery-single-big-1.jpg" alt="">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'gallery',
  method: {
    say: function (message) {
      alert(message)
    }
  }
}
</script>

<style lang="scss" scoped>
    .gallery-cover{
        color:black;
        min-height:300px;
    padding:0;margin:0;
    background:black;

    .row{
        margin:0;
        .img-cover{
            padding:0;
            position: relative;
            min-height:400px;
        }
    }
        .img-box{
            position: absolute;
                height: 100%;
    overflow: hidden;
    z-index:3;
            img{
                 -moz-transition: all 0.3s;
                                -webkit-transition: all 0.2s;
                                transition: all 0.2s
            }
            img:hover{
                cursor: pointer;
                -moz-transform: scale(1.1);
                        -webkit-transform: scale(1.1);
                        transform: scale(1.1)
            }
        }

        .bg-img-box{
            cursor: pointer;
            position: absolute;
            background: rgba(0, 0, 0, .5);
            width: 100%;
            height: 100%;
            top: 0;
            transition: all .3s;
            z-index:3;

            div{
                color:white;
                position: absolute;
                bottom: 0;
                width: 100%;
                padding: 0px 0px 35px 35px;
                text-align: left;

                span:first-child{
                    font-size:25px;
                }
            }
        }
    }
</style>
