<script>
	import Ingredients from "../components/Ingredients.svelte";
    import People from "../components/People.svelte";

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
        transition: background-color 0.1s ease-in-out;
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
        margin: 20px 0px 10px 0px;
        white-space: nowrap;
        scrollbar-width: none;
    }
    .carousel::-webkit-scrollbar {
        display: none;
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
        line-height: 1.3rem;
        font-size: 1.4rem;
        margin: 0px;
        margin-left: 0.75rem;
        width: 60%;
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
        min-height: 4  00px;
        margin-right: 1rem;
        padding: 0.5rem;
    }
    .product > div {
        white-space: normal;
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
        bottom: 100px;
        left: 10px;
    }
    .multiplier-text {
        color: white;
        position: absolute;
        bottom: 85px;
        left: 27.5px;
        font-size: 2rem;
        font-family: NowAltBold;
    }
    .buy-pill {
        text-decoration: none;
        color: white;
        background-color: rgba(60, 158, 54, 0.8);
        border: rgba(27, 111, 22, 0.8) 2px solid;
        border-radius: 30px;
        padding: 0.9rem 0.75rem 0.9rem 0.75rem;
        font-family: NowAltMedium;
        font-size: 0.75rem;
        transition: background-color 0.1s;
        width: 65%;
        display: inline-block;
        margin-top: 30px;
        margin-bottom: 10px;
    }

    .content {
        margin-left: 0.75rem;
        font-family: NowAltRegular;
    }
    .content-p {
        font-family: NowAltLight;
        line-height: 1.5rem;
    }
    .c-white {
        background-color: #fff;
    }
    #additives-header {
        font-family: NowAltMedium;
    }
    .row {
        margin: 0;
    }
    .text-center {
        text-align: center;
    }
    .free-section {
        margin-bottom: 5px;
    }
    .block-icon {
        height: 32px;
    }
    .superfood-title {
        font-family: 'Bodoni Moda', serif;
        font-size: 1.8rem;
        margin-top: 20px;
        margin-left: 0.75rem;
    }
    #sup-p {
        padding-left: 1rem;
        padding-right: 1rem;
        font-family: NowAltLight;
        line-height: 2.5rem;
        text-align: center;
        margin-top: -1rem;
        font-size: 0.9rem;
    }
    .sup-item {
        text-align: center;
        margin-top: 10px;
    }
    .sup-item > img {
        width: 35%;
    }
    .sup-item > h4 {
        font-family: NowAltBold;
        font-size: 1.3rem;
        width: 60%;
        margin-left: auto;
        margin-right: auto;
    }
    .sup-item > p {
        font-family: NowAltLight;
        line-height: 2rem;
        padding-left: 10px;
        padding-right: 10px;
    }

    .mid-banner {
        background-image: url('/images/home/mid-banner.png');
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        height: 125px;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    #banner-button {
        text-decoration: none;
        color: white;
        background-color: rgba(60, 158, 54, 0.8);
        border: rgba(27, 111, 22, 0.8) 3px solid;
        border-radius: 25px;
        padding: 0.5rem 0.75rem;
        font-family: NowAltMedium;
        font-size: 0.75rem;
        transition: background-color 0.1s ease-in-out;
    }
    #banner-button:hover, #banner-button:focus, #banner-button:focus-within {
        background-color: rgba(48, 126, 43, 0.8);
    }
    .customers {
        margin-top: 10px;
    }
    .star {
        width: 30px;
        padding: 0px;
        margin-left: 2.5px;
        margin-right: 2.5px;
    }
    .star-row {
        display: flex;
        justify-content: center;
    }
    .review-col {
        font-family: NowAltLight;
        line-height: 2rem;
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
    <div class="content">
        <div class="row">
            <div class="col-12 col-md-6">
                <h3 id="additives-header">NO ARTIFICIAL ADDITIVES</h3>
                <p class="content-p">No Herbicides or Pesticides, No GMO, No Artificial Colors, Flavors, Preservatives or Sweeteners.</p>
            </div>
            <div class="col-12 col-md-6">
                <div class="row text-center">
                    <div class="col-6 col-md-4 free-section">
                        <img src="/images/home/block.svg" alt="Red blocked icon" class="block-icon">
                        <p>GLUTEN FREE</p>
                    </div>
                    <div class="col-6 col-md-4 free-section">
                        <img src="/images/home/vegan-tick.svg" alt="Red blocked icon" class="block-icon">
                        <p>VEGAN</p>
                    </div>
                    <div class="col-6 col-md-4 free-section">
                        <img src="/images/home/block.svg" alt="Red blocked icon" class="block-icon">
                        <p>NUT FREE</p>
                    </div>
                    <div class="col-6 col-md-4 free-section">
                        <img src="/images/home/block.svg" alt="Red blocked icon" class="block-icon">
                        <p>NO GMO</p>
                    </div>
                    <div class="col-6 col-md-4 free-section">
                        <img src="/images/home/block.svg" alt="Red blocked icon" class="block-icon">
                        <p>DAIRY FREE</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="c-white">
        <div class="row">
            <div class="col-12">
                <h2 class="superfood-title">Açaí Berry is more than just a Superfood!</h2>
            </div>
        </div>
        <div class="row">
            <div class="col-12" id="sup-p">
                <p>Acai berries are packed full of nutrients that have unmatched benefits for your overall health & wellbeing. One daily serving provides an excellent source for Vitamin A, Vitamin C  & Vitamin D</p>
            </div>
        </div>
        <div class="row">
            <div class="sup-item">
                <img src="/images/home/increasedenergy.svg" alt="Increased Energy Purple Heart">
                <h4>INCREASED ENERGY</h4>
                <p>Contains antioxidants, monounsaturated fats , iron, calcium, fiber, vitamin A, & anthocyanins keep you full and energized  throughout the day</p>
            </div>
        </div>
        <div class="mid-banner">
            <a href="/shop" id="banner-button">
                Get Your ACAI
            </a>
        </div>
        <div class="customers">
            <div class="row">
                <div class="col-12 text-center">
                    <h2 class="superfood-title">5 Stars from over 16,000 Customers</h2>
                </div>
            </div>
            <div class="row star-row">
                <img src="/images/home/star.svg" alt="" class="star">
                <img src="/images/home/star.svg" alt="" class="star">
                <img src="/images/home/star.svg" alt="" class="star">
                <img src="/images/home/star.svg" alt="" class="star">
                <img src="/images/home/star.svg" alt="" class="star">
            </div>
            <div class="row">
                <div class="col-12 review-col text-center">
                    <p>“Tasty organic coffee flavour and great atmosphere. Amazing staff, however the place is small and pretty pricy for a bowl however the best yet acai bowl I tried.”</p>
                    <p>-Richard Barrett</p>
                </div>
            </div>
        </div>
    </div>
</div>
<Ingredients></Ingredients>
<People></People>