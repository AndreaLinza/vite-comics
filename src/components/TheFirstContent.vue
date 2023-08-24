<script>

export default {

};
</script>

<template>
    <section>
        <div class="jumbo position-relative">

            <div class="container">

                <span class="square text-uppercase">
                    current series
                </span>
            </div>
            
        </div>
    </section>
</template>

<style scoped lang="scss">
@use "../styles/partials/variables" as *;

section {
    font-family: $font-primary;
    background-color: #24201F;
        .jumbo{
            background-image: url('../assets/img/jumbotron.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            height: 400px;


            .square{
                font-weight: 600;
                background-color: $color-primary;
                color:white;
                display: flex;
                justify-content: center;
                align-items: center;
                height: 50px;
                width: 200px;
                position: absolute;
                bottom: -25px;
                left: 10;
                padding: 1rem;
            }
        }

    
}
</style>