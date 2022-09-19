<template>
    <div class="row">
        <div class="col-xs-12 col-sm-6 pb-5" v-bind:class="{ 'order-3': isLargeScreen, 'order-1': !isLargeScreen }">
            <div class="d-flex align-items-center">
                <img src="../assets/row-4-image.png" class="img-fluid" />
            </div>
        </div>
        <div class="col-xs-12 col-sm-6 pb-5 order-2">
            <div class="h-100 d-flex align-items-center">
                <div>
                    <span class="my-font-1">
                        Lorem ipsum dolor sit amet consectetur 
                    </span>
                    <br />
                    <span class="my-font-2">
                        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Suscipit nemo hic quos, ab, dolor aperiam nobis cum est eos error ipsum, voluptate culpa nesciunt delectus iste?
                    </span>
                    <br />
                    <button class="btn btn-dark mt-2" style="width: 170px;">Learn More</button>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .my-font-1{
        font-family: 'Crimson Text';
        font-size: 40px;
        font-weight: bold ;
    }

    .my-font-2{
        font-family: 'Work Sans';
        font-size: 15px;
    }
</style>

<script>
    export default {
        name: "Row4",
        props:{
            isLargeScreen: Boolean,
        }
    }
</script>