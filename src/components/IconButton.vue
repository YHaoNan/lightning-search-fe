<template>
    <button class="icon-button" :style="{color: color,backgroundColor: backgroundColor}">
        <img :src="icon">
        <slot></slot>
    </button>

</template>

<script>
    export default {
        name: "IconButton",
        props: {
            "color":{
                require: false,
                default: "#fff"
            },
            "icon":{
                require: true
            },
            "backgroundColor":{
                require: false,
                default: "#333"
            }
        },
        datas () {
        },
    }
</script>

<style scoped>
    .icon-button{
        border: none;
        box-shadow: none;
        font-weight: bold;
        padding: 10px 15px;
        display: inline-block;
        height: 50px;
        outline: none;
        border-radius: 5px;
        box-shadow: 0px 5px 10px rgb(0, 0, 0, 0.12);
        margin: 10px;
    }
    .icon-button:active{
        outline: none;
    }
    .icon-button img{
        display: inline-block;
        vertical-align: middle;
        width: 1.6em;
        margin-right: 10px;
    }

</style>