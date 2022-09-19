<template>
    <div class="row">
        <div class="col-xs-12 col-sm-6 py-2" v-bind:class="{ 'text-start': isLargeScreen, 'text-center': !isLargeScreen }">
            <img src="../assets/footer-image.png" />
        </div>

        <div class="col-xs-12 col-sm-6 py-2" v-bind:class="{ 'text-end': isLargeScreen, 'text-center': !isLargeScreen }">
            <span class="my-font-1">© Start, 2022. All rights reserved.</span>
        </div>
    </div>
</template>

<style scoped>
    .my-font-1{
        font-family: 'Work Sans';
        font-size: 20px;
        color: #FFFFFF;
    }
</style>

<script>
    export default {
        name: "Row5",
        props:{
            isLargeScreen: Boolean,
        }
    }
</script>