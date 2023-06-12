<script>

</script>

<style>
    .hero {
        min-height: 30vh;
        background-image: url('/images/home/landing-image.png');
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    #hero-button {
        text-decoration: none;
        color: white;
        background-color: rgba(60, 158, 54, 0.8);
        
        border: rgba(27, 111, 22, 0.8) 2px solid;
        border-radius: 5px;
        padding: 1rem 0.75rem 1rem 0.75rem;
        font-family: NowAltMedium;
        font-size: 0.75rem;
        transition: background-color 0.1s;
    }
    #hero-button:hover, #hero-button:focus, #hero-button:focus-within {
        background-color: rgba(48, 126, 43, 0.8);
    }
    .benefits{
        min-height: 30vh;
        background-color: #50253D;
    }
    #benefits-title {
        margin: 0px;
        margin-bottom: 0.5rem;
        padding: 1rem 0.75rem 0rem 0.75rem;
        font-size: 1.7rem;
        font-family: 'Cormorant Garamond', serif;
        font-weight: 500;
        color: white;

    }
    /*Carousel */
    .carousel-container {
        width: 100%;
        display: block;
        overflow: hidden;
    }
    .carousel {
        display: block;
        width: 100%;
        min-height: 225px;
        overflow-x: scroll;
        margin: 20px 0px 20px 0px;
        white-space: nowrap;
    }
    .item {
        display: inline-block;
        width: 65%;
        position: relative;
        min-height: 200px;
        margin-right: 1rem;
    }
    .item > div {
        white-space: normal;
        position: absolute;
        font-family: NowAltRegular;
        text-align: center;
    }
    .item > div > h4 {
        color: white;
    }
    .item > div > p {
        max-width: 25ch;
        color: white;
        font-size: 0.75rem;
    }
    .first {
        margin-left: 1rem;
    }
    .last {
        margin-right: 0px;
    }
    .carousel-icon {
        height: 55px;
    }
    /*End Carousel*/

    .main {
        background-color: #F9F2F6;
        min-height: 500px;
    }
    #quote-p {
        text-align: center;
        line-height: 1rem;
        margin: 0px;
        width: 50%;
        padding-top: 20px;
    }
    .bold-block {
        font-weight: bold;
        font-family: NowAltMedium;
    }
    #quote-exp {
        font-family: NowAltLight;
        line-height: 1.5rem;
        font-size: 0.8rem;
        padding: 0rem 1rem 0rem 1rem;
    }
    .product {
        display: inline-block;
        width: 60%;
        position: relative;
        background-color: white;
        border-radius: 5px;
        min-height: 400px;
        margin-right: 1rem;
        padding: 0.5rem;
    }
    .product > div {
        white-space: normal;
        position: absolute;
        font-family: NowAltRegular;
        text-align: center;
        width: 100%;
    }
    .product-img-container {
        text-align: center;
        background-image: url('/images/home/berry-tub.png');
        background-repeat: no-repeat;
        background-size: contain;
        width: 90%;
        min-height: 200px;
    }
    .multiplier-img {
        width: 20vw;
        position: absolute;
        bottom: 70px;
        left: 10px;
    }
    .multiplier-text {
        color: white;
        position: absolute;
        bottom: 60px;
        left: 30px;
        font-size: 2rem;
        font-family: NowAltBold;
    }
    .buy-pill {
        text-decoration: none;
        color: white;
        background-color: rgba(60, 158, 54, 0.8);
        border: rgba(27, 111, 22, 0.8) 2px solid;
        border-radius: 30px;
        padding: 1rem 0.75rem 1rem 0.75rem;
        font-family: NowAltMedium;
        font-size: 0.75rem;
        transition: background-color 0.1s;
        width: 60%;
        display: inline-block;
        margin-top: 30px;
    }
</style>

<div class="hero">
    <a href="/shop" id="hero-button">
        GET YOUR ACAI
    </a>
</div>
<div class="benefits">
    <h2 id="benefits-title">Some of the many benefits of eating Acai daily</h2>
    <div class="carousel-container">
        <div class="carousel">
            <div class="item first">
                <div>
                    <img src="/images/home/heart.svg" alt="Heart" class="carousel-icon">
                    <h4>PROTECT YOUR HEART</h4>
                    <p>
                        A high Vitamin C content of this tiny berry as well as its phenolic compounds have been shown to help protect against cardiovascular disease
                    </p>
                </div>
            </div>
            <div class="item">
                <div>
                    <img src="/images/home/energy.svg" alt="Energy" class="carousel-icon">
                    <h4>INCREASED ENERGY</h4>
                    <p>
                        Acai delivers a healthy dose of antioxidants, monounsaturated fats, iron, calcium, fibre, Vitamin A & anthocyanins, keeps your energy-levels high throughout the day
                    </p>
                </div>
            </div>
            <div class="item">
                <div>
                    <img src="/images/home/blood.svg" alt="Blood" class="carousel-icon">
                    <h4>INCREASED BLOOD FLOW</h4>
                    <p>
                        Acai berries are packed full of nutrients shown to help blood circulation, warding off various ailments and establishing better blow flow
                    </p>
                </div>
            </div>
            <div class="item last">
                <div>
                    <img src="/images/home/complexion.svg" alt="Complexion" class="carousel-icon">
                    <h4>A BETTER COMPLEXION</h4>
                    <p>
                        Powerful polyphenol antioxidants help to fight free radicals and oxidative stress, which can help slow down the aging process whilst maintaining healthy skin, hair and nails
                    </p>
                </div>
            </div>
        </div>
    </div>
</div>
<div class="main">
    <div class="quote">
        <p id="quote-p">
            <span class="bold-block">"Straight from</span><br><i>the amazon rainforest</i><br><span class="bold-block">to you"</span>
        </p>
        <p id="quote-exp">
            Boost your breakfast, enhance your pre-workout snack or treat yourself to a delicious desert with our powerful, great-tasting,  & ready-to-eat frozen Acai Berry. <i>Choose the right size tubs for you:</i>
        </p>
    </div>
    <div class="carousel-container">
        <div class="carousel">
            <div class="product first">
                <div>
                    <p class="product-title">6 x Acai Berry tubs - 200ml</p>
                    <p class="product-price">£23.94</p>
                    <div class="product-img-container">
                        <img src="/images/home/product-multiplier.png" alt="Multi" class="multiplier-img">
                        <p class="multiplier-text">6x</p>
                    </div>
                    <a href="#" class="buy-pill">BUY NOW</a>
                </div>
            </div>
            <div class="product">
                <div>
                    <div>
                        <p class="product-title">12 x Acai Berry tubs - 200ml</p>
                        <p class="product-price">£47.88</p>
                        <div class="product-img-container">
                            <img src="/images/home/product-multiplier.png" alt="Multi" class="multiplier-img">
                            <p class="multiplier-text">12x</p>
                        </div>
                        <a href="#" class="buy-pill">BUY NOW</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>