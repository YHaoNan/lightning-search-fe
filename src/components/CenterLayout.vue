<template>
    <div class="center-layout">
        <slot></slot>
    </div>
</template>

<script>
    export default {
        name: "CenterLayout"
    }
</script>

<style scoped>
    .center-layout{
        position: absolute;
        top: 50%;
        width: 100%;
        text-align: center;
        transform: translateY(-50%);
    }

</style>