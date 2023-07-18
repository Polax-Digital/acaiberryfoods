<style>
    footer {
        background-image: url("/images/footer/background.png");
        background-size: cover;
        background-position: center;
        padding: 6rem;
    }
    a {
        font-family: "Now Alt";
        font-size: 15px;
        font-style: normal;
        font-weight: 500;
        line-height: normal;
        color: #fff;
        text-decoration: none;
        text-transform: uppercase;
    }
    a:hover {
        text-decoration: underline;
    }
    .nav {
        padding: 0 4rem;
        margin-bottom: 5rem;
    }
    span p {
        margin: 0;
        color: #FFF;
        font-family: "Now Alt";
        font-size: 15px;
        font-style: normal;
        font-weight: 600;
        line-height: 40px;
        text-transform: uppercase;
    }
    .email {
        text-transform: lowercase;
    }
    .disclaimer {
        border: 1px solid #fff;
        padding: 10px;
        color: #fff;
        font-family: "Now Alt";
        font-size: 11px;
        font-style: normal;
        font-weight: 400;
        line-height: normal;
    }
    .disclaimer-2 {
        color: #fff;
        font-family: "Now Alt";
        font-size: 8px;
        font-style: normal;
        font-weight: 400;
        line-height: 19px;
        margin-bottom: 2rem;
    }
    .pptc {
        color: #fff;
        font-family: "Now Alt";
        font-size: 13px;
        font-style: normal;
        font-weight: 400;
        line-height: 20px;
        text-decoration: underline;
        text-transform: capitalize;
        margin: 0 1rem;
    }
    h4 {
        color: #fff;
        font-family: "Now Alt";
        font-size: 19px;
        font-style: normal;
        font-weight: 600;
        line-height: normal;
        margin: 0;
    }
    .contact {
        padding-left: 3rem;
    }
    .contact p {
        color: #fff;
        font-family: "Now Alt";
        font-size: 12px;
        font-style: normal;
        font-weight: 400;
        line-height: normal;
    }
    .contact a {
        margin: 0 1.5rem;
    }
    form {
        margin-right: 10rem;
        margin-bottom: 1rem;
    }
    .form-box {
        background-color: #fff;
        border-radius: 39px;
        padding: 1rem;
    }
    input, button {
        background-color: #fff;
        border: none;
        outline: none;
        color: #000;
        font-family: "Now Alt";
        font-size: 10px;
        font-style: normal;
        font-weight: 300;
        line-height: 20px;
    }
    input {
        width: 100%;
        height: 100%;;
    }
    input:focus {
        outline: none;
    }
    button:hover {
        cursor: pointer;
    }
</style>

<footer>
    <div class="row">
        <div class="col-8">
            <div class="row nav">
                <div class="col-2">
                    <a href="/shop">Shop</a>
                </div>
                <div class="col-2">
                    <a href="/about-us">About Us</a>
                </div>
                <div class="col-2">
                    <a href="/stores">Stores</a>
                </div>
                <div class="col-2">
                    <a href="/blog">Blog</a>
                </div>
                <div class="col-4">
                    <span><p>Contact Us</p></span>
                    <a href="mailto:info@acaiberryfoods.com" class="email">info@acaiberryfoods.com</a>
                </div>
            </div>
            <div class="row">
                <div class="col-3">
                    <img src="/images/header/acai-logo.svg" alt="Acai Logo" id="logo">
                </div>
                <div class="col-9">
                    <div class="disclaimer">
                        <p>* This product is not intended to diagnose, treat, cure or prevent any disease.</p>
                    </div>
                    <p class="disclaimer-2">Information on this site is provided for informational purposes only. It is not meant to substitute for medical advice from your physician or other medical professional. You should not use the information contained herein for diagnosing or treating a health problem or disease, or prescribing any medication. Carefully read all product documentation. If you have or suspect that you have a medical problem, promptly contact your regular health care provider.</p>
                    <a href="/privacy-policy" class="pptc">Privacy</a>
                    <a href="/terms-conditions" class="pptc">Terms & Conditions</a>
                </div>
            </div>
        </div>
        <div class="col-4 contact">
            <h4>Connect</h4>
            <p>Join Our Newsletter</p>

            <form action="">
                <div class="form-box">
                    <div class="row">
                        <div class="col-10">
                            <input required type="email" name="email" id="email" placeholder="Your Email">
                        </div>
                        <div class="col-2">
                            <button type="submit">
                                <svg xmlns="http://www.w3.org/2000/svg" width="33" height="23" viewBox="0 0 33 23" fill="none">
                                    <path d="M1.73242 9.95117C0.903995 9.95117 0.232422 10.6227 0.232422 11.4512C0.232422 12.2796 0.903995 12.9512 1.73242 12.9512V9.95117ZM32.4546 12.5118C33.0404 11.926 33.0404 10.9763 32.4546 10.3905L22.9087 0.84457C22.3229 0.258783 21.3731 0.258783 20.7874 0.84457C20.2016 1.43036 20.2016 2.3801 20.7874 2.96589L29.2726 11.4512L20.7874 19.9365C20.2016 20.5222 20.2016 21.472 20.7874 22.0578C21.3731 22.6436 22.3229 22.6436 22.9087 22.0578L32.4546 12.5118ZM1.73242 12.9512H31.394V9.95117H1.73242V12.9512Z" fill="black"/>
                                    </svg>
                            </button>
                        </div>
                    </div>
                </div>
                
            </form>

            <a href="https://www.instagram.com/acaiberryfoods/"><img src="/images/footer/insta.svg" alt="Instagram"></a>
            <a href="https://www.facebook.com/acaiberryfoods"><img src="/images/footer/fb.svg" alt="Facebook"></a>
            <a href="https://www.tiktok.com/@acaiberryfoods"><img src="/images/footer/tiktok.svg" alt="TikTok"></a>
        </div>
    </div>
</footer>