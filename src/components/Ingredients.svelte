<script>
    /**
	 * @type {any}
	 */
    let screenSize;
</script>

<style>
    .bod-f {
        font-family: 'Bodoni Moda', serif;
    }
    .quality-con {
        display: flex;
        align-items: center;
        color: white;
    }
    .quality-con > h4 {
        font-family: NowAltBold;
        margin: 0px;
        padding-top: 15px;
        padding-left: 5px;
    }
    .qual-p {
        font-family: NowAltLight;
        line-height: 30px;
        color: white;
        margin-bottom: 20px;
    }
    .nutrition-pill {
        color: white;
        text-decoration: none;
        padding: 15px 23px 15px 23px;
        border-radius: 50px;
        background-color: rgba(60, 158, 54, 0.8);
        border: rgba(27, 111, 22, 0.8) 3px solid;
        font-family: NowAltRegular;
        margin-left: 22px;
        font-size: 14px;
        transition: background-color 0.1s ease-in-out;
    }
    .nutrition-pill:hover, .nutrition-pill:focus, .nutrition-pill:focus-within {
        background-color: rgba(48, 126, 43, 0.8);
    }
    .ig-con {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 19px;
        border: #F5D5E8 3px solid;
        border-radius: 15px;
        margin: 18px 35px 0px 35px;
    }
    .ig-container {
        background: #50253D;
        color: white;
    }
    .img-container > .row {
        margin: 0px;
    }
    @media only screen and (max-width: 767px) {
        .ing-container {
            height: 520px;
        }
        .img-container {
            height: 320px;
            background:linear-gradient( rgba(80, 37, 61, 0.7) 100%, rgba(80, 37, 61, 0.7)100%),url('/images/ingredients/ing-bg-mobile.png');
            background-repeat: no-repeat;
            background-size: cover;
        }
        .ig-container {
            height: 200px;
        }
        .img-p {
            padding-left: 22px;
            padding-right: 22px;
            color: white;
            font-size: 1rem;
            margin-top: 20px;
        }
        .tick {
            width: 25px;
            padding-left: 22px;
            margin-top: 10px;
        }
        .qual-p {
            font-size: 12px;
            padding-left: 30px;
            padding-right: 30px;
        }
        .ig-con > span {
            font-family: NowAltLight;
            font-size: 15px;
        }
        .ig-con > img {
            height: 50px;
        }
        .js {
            display: flex;
            justify-items: center;
            flex-direction: column;
        }
        .join {
            font-family: NowAltLight;
            font-size: 10px;
            margin-top: 25px;
            margin-left: 35px;
        }
        .hashtag {
            font-family: 'Bodoni Moda', serif;
            font-size: 25px;
            margin-left: 35px;
        }
    }
</style>
<svelte:window bind:innerWidth={screenSize} />
<div class="ing-container">
    <div class="img-container">
        <div class="row">
            <div class="col-12 col-md-6 bod-f">
                <p class="img-p">
                    Acai Berries are packed full of nutrients,
                    delivering unmatched benefits for your
                    overall health and wellbeing.
                </p>
            </div>
            <div class="col-12 col-md-6 bod-f">
                <div class="quality-con">
                    <img src="/images/ingredients/tick.svg" alt="" class="tick">
                    <h4>QUALITY INGREDIENTS</h4>
                </div>
                <p class="qual-p">
                    We only use 100% fresh Acai Berries in every tub with no nasty ingredients. Straight from the Amazon Rainforest to your bowl!
                </p>
                <a href="#" class="nutrition-pill">Full Nutrition Values</a>
            </div>
        </div>
    </div>
    <div class="ig-container">
        {#if screenSize > 767}
        <div class="row">
            <div class="col-12 col-md-6 js">
                <span class="join">JOIN US</span>
                <span class="hashtag">#ACAIBERRYFOODS</span>
            </div>
            <div class="col-12 col-md-6">
                <div class="ig-con">
                    <img src="/images/ingredients/ig.svg" alt="" class="ig-logo">
                    <span>@acaiberryfoods</span>
                </div>
            </div>
        </div>
        {:else}
        <div class="row">
            <div class="col-12 col-md-6">
                <div class="ig-con">
                    <img src="/images/ingredients/ig.svg" alt="" class="ig-logo">
                    <span>@acaiberryfoods</span>
                </div>
            </div>
            <div class="col-12 col-md-6 js">
                <span class="join">JOIN US</span>
                <span class="hashtag">#ACAIBERRYFOODS</span>
            </div>
        </div>
        {/if}
    </div>
</div>