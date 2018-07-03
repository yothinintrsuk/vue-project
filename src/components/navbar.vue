<template>
    <div class="nav-body">
            <div class="nav-wrapper">
                    <div class="nav">
                    <div class="logo">
                    <a href="#">
                        <img src="../assets/logo/logo-light.png" alt="">
                    </a>
                    </div>
                    <div class="menu">
                        <ul>
                            <li>Product</li>
                            <li>Tutorials</li>
                            <li>Contact us</li>
                        </ul>
                    </div>
                </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>

<style lang="scss" scoped>
  .nav-body{
      position:fixed;
    //   background:black;
      z-index:99;
      width:100%;
  }
.nav-wrapper{
  max-width:1440px;
  margin-left:auto;
  margin-right:auto;
//   border:1px solid gray;
  z-index:10;
  .nav{
        .logo {
            float:left;
            width: 50%;
            text-align: left;
            a{
                img{
                    max-height: 50px;
                    max-width: 100%;
                    height: auto;
                }
            }
        }
        .menu {
            float:right;
            width: 50%;
            text-align: right;
            ul{
                list-style: none;
                margin:0;
                padding:0;
                li{
                    display: inline-block;
                    padding: 30px 0;
                    vertical-align: middle;
                    color:white;
                }
            }
        }
  }
}
</style>
