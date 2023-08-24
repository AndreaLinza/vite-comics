<script>
export default {
    data() {
        return {
            footerList: [
                {
                    title: 'DC COMICS',
                    credits: [
                        'Character',
                        'Comics',
                        'Movies',
                        'TV',
                        'Games',
                        'Videos',
                        'News',
                    ],
                },
                {
                    title: 'SHOP',
                    credits: ['Shop DC', 'Shop DC Collectibles'],
                },
                {
                    title: 'DC',
                    credits: [
                        'Terms of Use',
                        'Privacy policy (New)',
                        'Ad Choices',
                        'Advertising',
                        'Jobs',
                        'Subscriptioons',
                        'Talent WorkShops',
                        'CPSC Certificates',
                        'Ratings',
                        'Shop Help',
                        'Contact US',
                    ],
                },
                {
                    title: 'SITES',
                    credits: [
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        'DC Power Visa',
                    ],
                },
            ],
        };
    },
    methods: {},
}

</script>

<template>
    <footer>
        <div class="container">
            <div class="d-flex flex-column flex-wrap w-25 pt-4">
                <div v-for="singleElement in footerList" class="pe-5">
                    <h3 class="title">{{ singleElement.title }}</h3>
                    <ul class="me-auto mb-2 mb-lg-0 list-unstyled text-white pb-3">
                        <li v-for="singleCredits in singleElement.credits" class="nav-item">
                            <a class="nav-link" href="#">{{singleCredits}}</a>
                        </li>
                    </ul>
                </div>

                <div class="container">
                    <img class="dc-logo" src="../assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>
        <div class="sign-banner">
            <div class="container d-flex justify-content-between">
                <div>
                    <button type="button" class="btn btn-outline-primary border-3 text-light fw-bold">SIGN-UP NOW!</button>
                </div>
                <div>
                    <span>FOLLOW US</span>
                    <a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a>
                    <a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a>
                    <a href="#"><img src="../assets/img/footer-youtube.png" alt=""></a>
                    <a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a>
                    <a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a>
                </div>



            </div>
        </div>

    </footer>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

footer {
    max-height: 400px;

    font-family: $font-primary;
    background-image: url("../assets/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    background-position: bottom;

    .container>div{
        max-height: 400px;
    }


    a {
        
        text-decoration: none;
        color: #949393;

        &:hover {
            color: white
        }
    }

    .title {
        font-size: 1.3rem;
        padding-bottom: .5rem;
        text-transform: uppercase;
        font-weight: 600;
        color: white;
    }

    .dc-logo {
        position: absolute;
        right: 10%;
        height: 60%;
        overflow: hidden;
        top: 30%;

    }

    .sign-banner {
        min-height: 120px;
        background-color: $color-banner;
        display: flex;
        align-items: center;
        position: relative;

        span {
            font-weight: 600;
            color: $color-primary;
            padding-right: 2rem;
        }

        a {
            padding: 0 .5rem;

        }
        img:hover{
            border-radius: 50%;
            background-color:white;
        }

        .btn {
            border-radius: 0;

            .btn-outline-primary {
                --bs-btn-color: $color-primary;
                --bs-btn-border-color: $color-primary;
                --bs-btn-hover-color: #fff;
                --bs-btn-hover-bg: $color-primary;
                --bs-btn-hover-border-color: $color-primary;
                --bs-btn-focus-shadow-rgb: 13, 110, 253;
                --bs-btn-active-color: #fff;
                --bs-btn-active-bg: $color-primary;
                --bs-btn-active-border-color: $color-primary;
                --bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
                --bs-btn-disabled-color: $color-primary;
                --bs-btn-disabled-bg: transparent;
                --bs-btn-disabled-border-color: $color-primary;
                --bs-gradient: none;
            }
        }
    }

}
</style>