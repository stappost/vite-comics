<script>
export default {
    name: "AppFooter",
    props: {
        links: Array
    }
}
</script>
<template lang="">
    <footer>

        <div class="bg_img">
            <div class="container">
                <div class="row">
                    <div class="col-12">
                        <div>
                            <h3 class="text_white">DC COMICS</h3>
                            <ul>
                                <li v-for="(item, index) in links" key="index">
                                <a href="item.url">{{item.name}}</a>
                                </li>
                            </ul>
                            <h3 class="text_white">SHOP</h3>
                            <ul>
                                <li><a href="#"> Shop DC </a></li>
                                <li><a href="#"> Shop DC collectibles </a></li>
                            </ul>
                        </div>
                        <div>
                            <h3 class="text_white">DC</h3>
                            <ul>
                                <li><a href="#"> Terms Of Use </a></li>
                                <li><a href="#"> Privacy policy (New) </a></li>
                                <li><a href="#"> Ad Choices </a></li>
                                <li><a href="#"> Advertising </a></li>
                                <li><a href="#"> Jobs </a></li>
                                <li><a href="#"> Subscriptions </a></li>
                                <li><a href="#"> Talent Workshop </a></li>
                                <li><a href="#"> CPSC Certificates </a></li>
                                <li><a href="#"> Rating </a></li>
                                <li><a href="#"> Shop Help </a></li>
                                <li><a href="#"> Contact Us </a></li>
                            </ul>
                        </div>
                        <div>
                            <h3 class="text_white">SITES</h3>
                            <ul>
                                <li><a href="#"> DC </a></li>
                                <li><a href="#"> MAD Magazine </a></li>
                                <li><a href="#"> DC Kids </a></li>
                                <li><a href="#"> DC Universe </a></li>
                                <li><a href="#"> DC Power Visa </a></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="bg_grey">
            <div class="container">
                <div class="row">
                    <div class="col-6">
                        <button>SIGN-UP NOW!</button>
                    </div>
                    <div class="col-6 text_right">
                        <span>FOLLOW US</span>
                        <a href="#">
                            <img src="../assets/img/footer-facebook.png" alt="facebook">
                        </a>
                        <a href="#">
                            <img src="../assets/img/footer-twitter.png" alt="twitter">
                        </a>
                        <a href="#">
                            <img src="../assets/img/footer-youtube.png" alt="youtube">
                        </a>
                        <a href="#">
                            <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                        </a>
                        <a href="#">
                            <img src="../assets/img/footer-periscope.png" alt="periscope">
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>
<style lang="scss" scoped>
@use '../styles/partials/variabiles' as *;

.bg_img {
    background-image: url('../assets/img/footer-bg.jpg');

    .text_white {
        color: #fff;
        margin: 20px 0;
    }

    ul {
        list-style: none;
        margin-bottom: 30px;

        li a {
            text-decoration: none;
            color: grey;
        }
    }

    .col-12 {
        display: flex;
        background-image: url('../assets/img/dc-logo-bg.png');
        background-position: right;
        background-repeat: no-repeat;

    }

}

.bg_grey {
    background-color: rgb(71, 71, 71);
    padding: 10px 0;

    .row {
        justify-content: space-between;
        align-items: center;
    }

    button {
        border: 2px solid $primary;
        color: white;
        padding: 5px;
        background-color: transparent;
    }

    .text_right {

        span {
            margin-right: 15px;
            color: $primary;
        }

        a {
            vertical-align: middle;
            margin: 0 5px;
        }
    }
}
</style>