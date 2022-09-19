<template>
    <div class="row">
        <div class="col-xs-12 col-sm-6 pb-5 px-2">
            <div class="d-flex align-items-center">
                <img src="../assets/row-3-image.png" class="img-fluid" />
            </div>
        </div>

        <div class="col-xs-12 col-sm-6 pb-5 px-2">
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
                    <div class="py-2">
                        <button class="btn btn-dark" style="width: 170px;">Learn More</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .my-font-1{
        font-family: 'Poppins';
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
        name: "Row3"
    }
</script>