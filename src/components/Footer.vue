<template>
    <footer>
        <section class="footer-top">

            <section class="wrapper">
                <div class="top-left">
                    <div class="menu">
                        <h3>dc comics</h3>
                        <ul>
                            <li><a href="">characters</a></li>
                            <li><a href="">comics</a></li>
                            <li><a href="">movies</a></li>
                            <li><a href="">tv</a></li>
                            <li><a href="">games</a></li>
                            <li><a href="">videos</a></li>
                            <li><a href="">news</a></li>
                        </ul>
                        <h3>shop</h3>
                        <ul>
                            <li><a href="">Shop DC</a></li>
                            <li><a href="">Shop DC Collectibles</a></li>
                        </ul>
                    </div>
                    <div class="menu">
                        <h3>dc</h3>
                        <ul>
                            <li><a href="">Terms Of Use</a></li>
                            <li><a href="">Privacy policy (New)</a></li>
                            <li><a href="">Ad Choices</a></li>
                            <li><a href="">Advertising</a></li>
                            <li><a href="">Jobs</a></li>
                            <li><a href="">Subscriptions</a></li>
                            <li><a href="">Talent Workshops</a></li>
                            <li><a href="">CPSC Certificates</a></li>
                            <li><a href="">Ratings</a></li>
                            <li><a href="">Shop Help</a></li>
                            <li><a href="">Contact Us</a></li>
                        </ul>
                    </div>
                    <div class="menu">
                        <h3>sites</h3>
                        <ul>
                            <li><a href="">DC</a></li>
                            <li><a href="">MAD Magazine</a></li>
                            <li><a href="">DC Kids</a></li>
                            <li><a href="">DC Universe</a></li>
                            <li><a href="">DC Power Visa</a></li>
                        </ul>
                    </div>
                </div>
                    
                <div class="top-right"></div>
            </section>
        </section>
        <section class="footer-bottom">
            <section class="wrapper">
                <div class="bottom-left">
                    <button>sign up now</button>
                </div>
                <div class="bottom-right">
                    <h3>follow us</h3>
                    <img src="../assets/images/footer-facebook.png" alt="facebook">
                    <img src="../assets/images/footer-twitter.png" alt="twitter">
                    <img src="../assets/images/footer-youtube.png" alt="youtube">
                    <img src="../assets/images/footer-pinterest.png" alt="pinterest">
                    <img src="../assets/images/footer-periscope.png" alt="periscope">
                </div>
            </section>
        </section>
        
            
    </footer>
</template>

<script>

export default {
    name: "Footer"
}

</script>

<style lang="scss" scope>

    @import "../style/Color.scss";
    footer {
        width: 100%;
    
    .wrapper {
        display: flex;
        width: 70%;
        height: 100%;
        margin: auto;
    }
    h3, h4 {
        text-align: left;
        font-size: 15px;
        color: $text-color;
        padding: 10px 0;
        text-transform: uppercase; 
    }
            .footer-top {
                display: flex;
                width: 100%;
                height: 100%;
                background-image: url(../assets/images/footer-bg.jpg);
                background-size: cover;
                flex-wrap: wrap;
                    
                    .top-left { 
                        display: flex;
                        flex-wrap: wrap;
                        width: 50%;
                        height: 100%;
                        padding-bottom: 50px;

                        .menu {
                            width: 130px;

                            h3:first-child {
                                padding: 50px 0 20px 0;
                            }
                            ul  {
                                list-style: none;

                                li {
                                text-align: left;
                                font-size: 10px;
                                margin: 5px 0;

                                    a {
                                        text-decoration: none;
                                        color: $color-list;

                                    }

                                }
                            }
                        }
                    
                    }

                    .top-right { 
                        width: 50%;
                        background-image: url(../assets/images/dc-logo-bg.png);
                        background-size: 90%;
                        background-repeat: no-repeat;
                        background-position-y: center;

                    }
            }
            
            .footer-bottom {
                width: 100%;
                height: 100px;
                background-color: $bg-footer;

                .bottom-left {
                    display: flex;
                    width: 50%;
                    height: 100%;
                    text-align: left;
                    align-items: center;

                    button {
                        text-transform: uppercase;
                        background-color: $bg-footer;
                        border: 1px solid $logo-color;
                        padding: 10px;
                        color: $text-color;
                    }
                }

                .bottom-right {
                    display: flex;
                    width: 50%;
                    height: 100%;
                    justify-content: flex-end;
                    align-items: center;
                    
                    h3 {
                        margin-right: 20px;
                        color: $logo-color;
                    }
                    img {
                        width: 25px;
                        margin: 0 5px;
                    }
                }
                

            }
    }
</style>