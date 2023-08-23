<script>
export default {};
</script>

<template>
    <header>
        <div class="container">
            <nav class="navbar navbar-expand-lg">

                <div>
                    <img src="../assets/img/dc-logo.png" alt="DC">
                </div>

                <div class="collapse navbar-collapse d-flex justify-content-end">
                    <ul class="navbar-nav">
                        <li class="nav-item">
                            <a class="nav-link text-uppercase" href="#">characters</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link text-uppercase" href="#">comics</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link text-uppercase" href="#">movies</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link text-uppercase" href="#">tv</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link text-uppercase" href="#">games</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link text-uppercase" href="#">collectibles</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link text-uppercase" href="#">video</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link text-uppercase" href="#">fans</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link text-uppercase" href="#">news</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link text-uppercase" href="#">shop</a>
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


        .nav-link {
            color: $color-text;
            border-radius: 0;
            border-bottom: 2px;

            &.hover {
                color: $color-primary;
                background-color: $color-primary;
            }
        }
    }
}
</style>