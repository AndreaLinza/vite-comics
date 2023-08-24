<script>


export default {
    props: {
        thumb: String,
        series: {
            type: String,
            required: true,
        },
    },


}

</script>


<template>
    

        <div class="card">
            <img :src="thumb" alt="...">
            <div class="card-body">
                <p class="card-text">{{ series }}</p>
            </div>
        </div>


</template>

<style lang="scss" scoped>


    .card {

        width: 100%;
        height: 100%;
        background-color: transparent;
        border: 0;
        border-radius: 0;
        color: white;

        img {
            width: 100%;
            object-fit: cover;
            aspect-ratio: 1/1;
        }
    }
</style>