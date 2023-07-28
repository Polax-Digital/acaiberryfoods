<script>
	import { page } from "$app/stores";

    console.log($page.url.pathname)

    

</script>

<style>
    header {
        background-color: #50253D;
        width: 100vw;
        max-height: 110px;
    }
    .container, .row {
        max-height: 110px;
        margin: 0 auto;
    }
    .promotion {
        background-color: #3C9E36;
        width: 100vw;
        text-align: center;
        padding: 12px;
    }
    .promotion p {
        color: #fff;
        font-family: "Now Alt";
        font-size: 15px;
        font-style: normal;
        font-weight: 500;
        line-height: normal;
        text-transform: uppercase;
        margin: 0;
    }
    #logo {
        width: 150px;
        position: relative;
        top: 14px;
    }
    #header-right {
        display: flex;
        align-items: center;
        justify-content: right;
        max-height: 110px;
    }
    #header-right > div {
        padding-left: 7px;
        padding-right: 7px;
    }
    #header-center {
        display: flex;
        align-items: center;
        max-height: 110px;
        text-align: center;
    }
    #header-center .row {
        margin: 0;
        width: 100%;
    }
    #cart {
        height: 20px;
    }
    #account {
        height: 20px;
    }
    #burger {
        height: 17px;
        display: none;
    }
    .left {
        margin-right: 5px;
    }
    .right {
        margin-left: 5px;
    }
    a {
        color: #fff;
        font-family: "Now Alt";
        font-size: 15px;
        font-style: normal;
        font-weight: 500;
        line-height: normal;
        text-transform: uppercase;
        text-decoration: none;
    }
    a:hover {
        text-decoration: underline;
    }
    .mobile-menu {
        display: none;
    }
    /* Media Queries */
    @media (max-width: 430px) {
        #header-center {
            display: none;
        }
        #account {
            display: none;
        }
        #burger {
            display: block;
        }
        .mobile-menu {
            
        }
    }
    @media (max-width: 768px) {
        #logo {
            width: 100px;
        }
        header, .container, #header-center, #header-right {
            height: 60px;
        }
        .container, header {
            margin: 0;
            max-width: 100%;
        }
        a {
            font-size: 11px;
        }
    }
</style>

<div class="promotion">
    <p>20% Off On Your First Order</p>
</div>
<header>
    <div class="container">
        <div class="row">
            <div class="col-lg-4 col-sm-3 col-6">
                <a href="/">
                    <img src="/images/header/acai-logo.svg" alt="Acai Logo" id="logo">
                </a>
            </div>
            <div class="col-lg-4 col-6" id="header-center">
                <div class="row">
                    <div class="col-3">
                        <a href="/shop">Shop</a>
                    </div>
                    <div class="col-3">
                        <a href="/about-us">About Us</a>
                    </div>
                    <div class="col-3">
                        <a href="/stores">Stores</a>
                    </div>
                    <div class="col-3">
                        <a href="/blog">Blog</a>
                    </div>
                </div>
            </div>
            <div class="col-lg-4 col-sm-3 col-6" id="header-right">
                <div class="left">
                    <a href="/">
                        <img src="/images/header/cart-icon.svg" alt="Cart Icon" id="cart">
                    </a>
                </div>
                <div class="right">
                    <a href="/">
                        <img src="/images/header/menu.svg" alt="Menu" id="burger">
                    </a>
                    <a href="/">
                        <img src="/images/header/account.svg" alt="Account" id="account">
                    </a>
                </div>
            </div>
        </div>
    </div>
</header>
<ul class="mobile-menu">
    <li>
        <a href="/shop">Shop</a>
    </li>
    <li>
        <a href="/about-us">About Us</a>
    </li>
    <li>
        <a href="/stores">Stores</a>
    </li>
    <li>
        <a href="/blog">Blog</a>
    </li>
</ul>