<style>
    .header {
        min-width: 100vw;
        height: 75vh;
        background-image: url("/images/about-us/header.png");
        background-size: cover;
        background-position: center;
    }
    .header-content {
        background-color: rgba(60, 158, 54, 0.6);
        color: #fff;
        text-align: center;
        width: 54vw;
        margin: 0 auto;
        padding: 50px;
        top: 8rem;
        position: relative;
    }
    .header-content small {
        font-family: "Now Alt";
        text-transform: uppercase;
        font-size: 15px;
    }
    .header-content p {
        font-family: 'Bodoni Moda', serif;
        font-size: 35px;
        line-height: 50px;
    }
    .page-content {
        width: 85%;
        margin: 0 auto;
        margin-bottom: 5rem;
        padding-top: 4rem;
    }
    .page-content p {
        font-family: "Now Alt";
        font-size: 20px;
        line-height: 50px;
        font-weight: 400;
        font-style: normal;
    }
    .page-content h2 {
        text-transform: uppercase;
    }
    .container {
        width: 627px;
        height: 3px;
        background-color: #3C9E36;
        position: relative;
        margin-bottom: 100px;
        left: 34px;
    }
    .circle {
        display: inline-block;
        vertical-align: left;
        width: 15px;
        height: 15px;
        background-color: #3C9E36;
        border: solid 1px #3C9E36;
        border-radius: 50%;
        position: absolute;
        top: -8px;
        left: -23px;
    }
    .container.inverse {
        left: -85px;
    }
    .circle.inverse {
        left: 101%;
    }
    #about, #acai {
        padding-top: 100px
    }
    #img-col-about {
        text-align: right;
    }
    .box {
        background: #3C9E36;
        border: 5px solid #1B6E16;
        width: 100%;
        text-align: center;
        margin: 5rem 0;
        border-radius: 20px;
        border-bottom-right-radius: 100px;
        color: #fff;
    }
    .box p {
        padding: 0 6rem;
        margin-top: 0;
        font-size: 20px;
    }
    .box h1 {
        font-weight: 400;
    }
    .fsde-container div {
        color: #fff;
        text-align: center;
        padding: 4rem;
    }
    .fsde-container h3 {
        font-size: 35px;
        font-family: "Now Alt";
        font-weight: 900;
        letter-spacing: 3.5px;
        margin: 0;
        text-transform: uppercase;
    }
    .fsde-container p {
        font-size: 20px;
        font-family: "Now Alt";
        line-height: 50px;
        margin: .5rem auto;
        max-width: 50%;
    }
    .development p {
        max-width: 60%;
    }
    .fairtrade, .social, .development, .environment {
        position: relative;
    }
    .fairtrade *, .social *, .development *, .environment * {
        position: relative;
    }
    .fairtrade::before, .social::before, .development::before, .environment::before {
        content: "";
        position: absolute;
        top: 0; left: 0;
        width: 100%; height: 100%;
        background-image: url("images/about-us/fairtrade.png");
        background-size: cover;
        background-position: center;
        filter: brightness(50%);
    }
    .social::before {
        background-image: url("images/about-us/social.png");
    }
    .development::before {
        background-image: url("images/about-us/development.png");
    }
    .environment::before {
        background-image: url("images/about-us/environment.png");
    }

    /* Media Queries */
    @media screen and (max-width: 768px) {
        .container {
            width: 80vw;
        }
        #img-col-about img, #img-col-acai img {
            width: 100%;
        }
    }
    @media screen and (max-width: 430px) {
        .header {
            height: 35vh;
        }
        .header-content {
            top: 5rem;
            padding: 1rem;
        }
        .header-content p {
            font-size: 11px;
            line-height: 15px;
        }
        .header-content small {
            font-size: 13px;
        }
        #about {
            padding-top: 0;
        }
        #acai {
            padding-top: 30px;
        }
        .page-content h1 {
            font-size: 20px;
        }
        .page-content p {
            font-size: 12px;
            line-height: 30px;
        }
        .container {
            margin-bottom: 0;
        }
        .box h1 {
            padding: 0 1rem;
        }
        .box p {
            padding: 0 1rem;
        }
        .fsde-container h3 {
            font-size: 20px;
            letter-spacing: 1.5px;
        }
        .fsde-container p {
            font-size: 12px;
            line-height: 15px;
            max-width: 80%;
        }
    }
</style>

<div class="header">
    <div class="header-content">
        <small>Our Mission</small>
        <p>Bringing the incredible benefits of Acai Berries straight from the Amazon Rainforest to your bowl!</p>
    </div>
</div>
<div class="page-content">
    <div class="row">
        <div class="col-lg-6" id="about">
            <div class="container">
                <div class="circle">
              
                </div>
              </div>
            <h2>About Us</h2>
            <p>Founded in 2017 Acai Berry Foods was created with the belief that everybody should be able to eat, enjoy, and benefit from this incredible superfood berry exactly as if they were in the heart of the Amazon Rainforest. We now deliver the freshest and more concentrated Acai product on the market, available to buy as a ready-made bowl from our 7 cafes around London or delivered straight to your door to create your own bowls at home.</p>
        </div>
        <div class="col-lg-6" id="img-col-about">
            <img src="/images/about-us/shop.png" alt="Acai Berry Shop">
        </div>
    </div>
    <div class="box">
        <h1>Time To See What All The Fuss Is About!</h1>
        <p>As the #1 ‘Acai Hotspot’ in London, it’s no surprise that our café’s often have a queue of customers around the building waiting in excitement to get their daily Acai. From delicious freshly made bowls loaded with healthy toppings to energising smoothies, our nutritious Acai Berry products have fast become a crowd favourite. By popular demand, we’re now offering you the ability to create your favourite bowls, smoothies and more at home with our tubs of ready-to-eat frozen Acai!</p>
    </div>
    <div class="row">
        <div class="col-lg-6" id="img-col-acai">
            <img src="/images/about-us/amazon.png" alt="Acai Berries">
        </div>
        <div class="col-lg-6" id="acai">
            <div class="container inverse">
                <div class="circle inverse">
              
                </div>
              </div>
            <h2>WHAT IS AÇAI?</h2>
            <p>Acai is a palm fruit which grows on the banks of the Amazon river in Brazil. It is small in size - smaller than a grape - and dark purple in colour. Acai consists of around 90% seed, covered in a small amount of pulp. Despite its small size, Acai packs a nutritional punch unlike any other food in the world, with enormous health benefits. Some researchers have called it the #1 Super Food in the World!</p>
        </div>
    </div>
</div>
<div class="fsde-container">
    <div class="fairtrade">
        <h3>Fairtrade</h3>
        <p>We guarantee that the farmers and producers we work with are getting our full support!</p>
    </div>
    <div class="social">
        <h3>Social</h3>
        <p>We make sure our workers decent working conditions. We directly support local workers' union.</p>
    </div>
    <div class="development">
        <h3>Development</h3>
        <p>We donate a meaningful percentage of our profits to local organisations as part of our efforts to give back and support the communities that we operate in.</p>
    </div>
    <div class="environment">
        <h3>Environment</h3>
        <p>Our production is totally sustainable, where natural resources involved cultivation our berries fully respected.</p>
    </div>
</div>