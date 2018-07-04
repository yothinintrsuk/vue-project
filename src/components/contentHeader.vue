<template>
    <div class="content-box-wrapper">
        <div class="content-background">
        </div>
        <div class="content-wrapper">
            <div class="content-inside">
                <h1>
The Coolest Photo Project I've Ever Created</h1>
                <p>
                    Fusce imperdiet, arcu non tempor aliquam, justo tortor cursus est, sed facilisis eros purus et felis. Sed eros sapien, iaculis eget gravida euismod, dapibus vitae turpis. Pellentesque men egestas odio mi, vitae egestas massa elementum ut. Cras dolor dui consequat ...
                </p>
            </div>
        </div>
        <div style="
            position: absolute;
            width: 100%;
            min-height: 500px;
            background: black;
            z-index: 3;
        ">
        </div>
    </div>
</template>

<script>
export default {
  name: 'contentHeader'
}
</script>

<style lang="scss" scoped>
.content-box-wrapper{
    min-height:500px;
}
    .content-background{
        position: absolute;
        width: 100%;
        min-height:500px;
        background-image:url('../assets/bg-header.jpg');
        opacity: 0.3; filter: alpha(opacity=30);
        background-position: center;
        z-index:4;
    }
    .content-wrapper{
        position: absolute;
         width: 100%;
        min-height:500px;
        vertical-align: middle;
        color:white;
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-align: center;
        -ms-flex-align: center;
        align-items: center;
        -webkit-box-pack: center;
        -ms-flex-pack: center;
        justify-content: center;
        z-index:5;
        .content-inside{
            width:1440px;
            text-align: left;
            h1{
                color:white;
                max-width: 45%;
                font-size: 50px;
                font-weight: 600;
            }
            p{
                color: #adadad;
    max-width: 45%;
    font-size: 16px;
            }
        }
    }
</style>
