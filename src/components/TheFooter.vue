<script>
export default {};
</script>

<template>
    <footer>
        <div class="container">
            <div class="d-flex pt-4">

                <div class="pe-5">
                    <h3 class="title">dc comics</h3>
                    <ul class="list-unstyled ">
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">Tv</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>

                    <h3 class="title pt-4">shop</h3>
                    <ul class="list-unstyled">
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>

                </div>

                <div class="pe-5">
                    <h3 class="title">dc</h3>
                    <ul class="list-unstyled">
                        <li><a href="#">Terms Of Use</a></li>
                        <li><a href="#">Privacy policy (New)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Rating</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>
                </div>

                <div>
                    <h3 class="title">sites</h3>
                    <ul class="list-unstyled">
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>
                </div>

                <div class="dc-logo">
                    <img src="../assets/img/dc-logo-bg.png" alt="">    
                </div>

            </div>
            <div>

            </div>
        </div>
    </footer>
</template>

<style scoped lang="scss">
@use "../styles/partials/variables" as *;

footer {
    font-family: $font-primary;
    padding-top: 2rem;
    padding-bottom: 7rem;
    background-image: url("../assets/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    background-position: bottom;
    

    a {
        text-decoration: none;
        color: #949393;
    }

    .title {
        font-size: 1.3rem;
        padding-bottom: .5rem;
        text-transform: uppercase;
        font-weight: 600;
        color: white;
    }

    .dc-logo{
        
        transform: translate(200px, -150px)
    }

}
</style>