<template>
    <div class="left-layout">
        <img id="banner" src="https://s2.ax1x.com/2019/11/07/MFX9Gd.png" alt="banner">
        <p class="title">像闪电一般的一键式搜书工具</p>
        <p class="button-group">
            <IconButton icon="https://s2.ax1x.com/2019/11/07/MF7Zad.png" background-color="#f3b03c">下载v1.0.0</IconButton>
            <IconButton icon="https://s2.ax1x.com/2019/11/07/MFbr59.png">去Gayhub</IconButton>
        </p>
    </div>
</template>

<script>
    import IconButton from './IconButton.vue'
    export default {
        name: "LeftLayout",
        components: {
            IconButton
        }
    }
</script>

<style scoped>
    .left-layout{
        display: inline-block;
        margin: 0 20px;
        margin-top: 40px;
    }
    #banner{
        max-width: 200px;
    }
    .title{
        font-family: '思源黑体','微软雅黑',sans-serif;
        font-weight: bold;
        font-size: 1.4em;
        color: #333;
    }
    .button-group{
        margin-top: 50px;
        margin-bottom: 50px;
    }

</style>