<script>
export default {
    
};
</script>

<template>
    <div class="container">
        <div class="banner-main z-1">
            <div>
                <img src="../assets/img/buy-comics-digital-comics.png" alt="digital-comics">
                <span>digital comics</span>
            </div>
            <div>
                <img src="../assets/img/buy-comics-merchandise.png" alt="dc-merchandise">
                <span>dc merchandise</span>

            </div>
            <div>
                <img src="../assets/img/buy-comics-subscriptions.png" alt="subscription">
                <span>subscription</span>

            </div>
            <div>
                <img src="../assets/img/buy-comics-shop-locator.png" alt="comic-shop">
                <span>comic shop locator</span>

            </div>
            <div>
                <img src="../assets/img/buy-dc-power-visa.svg" alt="dc-power" style="height: 50px;">
                <span>dc power visa</span>

            </div>
        </div>

    </div>
</template>

<style scoped lang="scss">
@use "../styles/partials/variables" as *;

div {
    display: flex;
    justify-content: center;
    align-items: center;

    img {
        height: 60px;
        margin-left: 3rem;

    }


    span {
        font-size: .8rem;
        display: flex;
        padding-left: 1rem;
        text-transform: uppercase;
        color: white;
    }
}

</style>