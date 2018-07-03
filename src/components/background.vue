<template>
    <div class="background-cover">

    </div>
</template>

<script>
export default {
  name: 'background'
}
</script>

<style lang="scss" scoped>
    .background-cover{
        position:absolute;
            background:rgba(0,0,0,.5);
            height:inherit;
            width:100vw;
            z-index:1;
            top:0;
            left:0;
    }
</style>
