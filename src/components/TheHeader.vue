<script>
export default {

    data(){
        return{
            headerList:[
                'Characters',
                'Comics',
                'Movies',
                'Tv',
                'Games',
                'Collectibles',
                'Video',
                'Fans',
                'News',
                'Shop'
            ]

        }
    }


};
</script>

<template>
    <header class="py-2">
        <div class="container">
            <nav class="navbar navbar-expand-lg">

                <div>
                    <img src="../assets/img/dc-logo.png" alt="DC">
                </div>

                <div class="collapse navbar-collapse d-flex justify-content-end">
                    <ul v-for="singleElement in headerList" class="navbar-nav">
                        <li class="nav-item">
                            <a class="nav-link text-uppercase" href="#">{{singleElement}}</a>
                        </li>
                    </ul>
                </div>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

header {
    font-family: $font-primary;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding-bottom: 1rem;

    img {
        width: 70px;
    }

    .navbar-nav {
        font-size: .8rem;
        font-weight: 600;


        a {
            color: $color-text;

            &:hover {
                color: $color-primary;              
                border-bottom: 1px solid $color-primary;
            }
        }
    }
}
</style>