<script >
export default{
}
</script>

<template>
    <footer>
        <section class="upper-footer">
            <div>
                <article id="dc-comics">
                <h2>
                   dc comics 
                </h2>
                <ul>
                    <li><a href="#">Characters</a></li>
                    <li><a href="#">Comics</a></li>
                    <li><a href="#">Movies</a></li>
                    <li><a href="#">Tv</a></li>
                    <li><a href="#">Games</a></li>
                    <li><a href="#">Videos</a></li>
                    <li><a href="#">News</a></li>

                </ul>
            </article>
            <article id="shop">
                <h2>
                    shop
                </h2>
                <ul>
                    <li><a href="#">Shop dc</a></li>
                    <li><a href="#">Shop dc collectibles</a></li>
                </ul>
            </article>
            </div>
            
            <article id="dc">
                <h2>
                    dc
                </h2>
                <ul>
                    <li><a href="#">Term Of Use</a></li>
                    <li><a href="#">Privacy policy (New)</a></li>
                    <li><a href="#">Ad Choices</a></li>
                    <li><a href="#">Advertising</a></li>
                    <li><a href="#">Jobs</a></li>
                    <li><a href="#"></a>Subscriptions</li>
                    <li><a href="#">Talent Workshops</a></li>
                    <li><a href="#">CPSC Certificates</a></li>
                    <li><a href="#">Ratings</a></li>
                    <li><a href="#">Shop Help</a></li>
                    <li><a href="#">Contact Us</a></li>
                </ul>
            </article>
            <article id="sites">
                <h2>
                    sites
                </h2>
                <ul>
                    <li><a href="#">DC</a></li>
                    <li><a href="#">MAD Magazine</a></li>
                    <li><a href="#">DC Kids</a></li>
                    <li><a href="#">Dc Universe</a></li>
                    <li><a href="#">DC Power Visa</a></li>
                </ul>
            </article>
            <img src="../assets/img/dc-logo-bg.png" alt="">

        </section>
        <section class="lower-footer">
            <button> Sign up now</button>
            <div>
                <h2>follow us</h2>
                <img src="../assets/img/footer-facebook.png" alt="facebook icon">
                <img src="../assets/img/footer-twitter.png" alt="twitter icon">
                <img src="../assets/img/footer-youtube.png" alt="youtube icon">
                <img src="../assets/img/footer-pinterest.png" alt="pinterest icon">
                <img src="../assets/img/footer-periscope.png" alt="periscope icon">
            </div>
        </section>
        
    </footer>
</template>

<style lang="scss" scoped>
    @use '../style/partials/variables' as *;
    @use '../style/partials/mixins' as *;

    footer{
        section.upper-footer{
        background-image: url(../assets/img/footer-bg.jpg);
        background-position: center;
        background-size: cover;
        @include flex (row, start, stretch );
            div{
                margin-left: 14rem;
            }
            article{
                padding: 3rem;
               
            }
            ul {
                padding-left: 0;
            }
            h2{
                text-transform: uppercase;
                font-size: 1.2rem;
                color:$white;
            }
            img{
                width: 25rem;
            }
        }

        section.lower-footer{
            padding-right: 15rem;

            @include flex (row, space-between , center);
            background-color: $footerBg;
                button{
                    background-color: transparent;
                    border: 2px solid blue;
                    color: $white;
                    text-transform: uppercase;
                    padding: 0.7rem;
                    margin: 1.8rem 0 1.8rem 16rem;
                }
                h2{
                    text-transform: uppercase;
                    font-size: 1.2rem;
                    color:blue;
                }
                div{
                    @include flex (row, center , center);

                    h2{
                        margin-right: 1rem;
                    }
                    img{
                        width: 25px;
                        margin: 0.4rem;
                    }
  
                }
        }
    
}
</style>