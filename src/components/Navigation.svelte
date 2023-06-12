<script>
	import { page } from "$app/stores";

    console.log($page.url.pathname)

</script>

<style>
    header {
        background-color: #50253D;
        width: 100vw;
        max-height: 60px;
    }
    .container, .row {
        padding: 0px;
        margin: 0px;
        max-height: 60px;
    }
    #logo {
        width: 100px;
        position: relative;
        top: 14px;
    }
    #header-right {
        display: flex;
        align-items: center;
        justify-content: right;
        max-height: 60px;
    }
    #header-right > div {
        padding-left: 7px;
        padding-right: 7px;
    }
    #cart {
        height: 20px;
    }
    #burger {
        height: 17px;
    }
    .left {
        margin-right: 5px;
    }
    .right {
        margin-left: 5px;
    }
    /* Media Queries */
    /* Small */
    @media (min-width: 576px) {
        
    }
    /* Medium */
    @media (min-width: 768px) {
        
    }
    /* Large */
    @media (min-width: 992px) {
        
    }
    /* XL */
    @media (min-width: 1200px) {
        
    }
    /* XXL */
    @media (min-width: 1400px) {
        
    }
    
    
</style>

<header>
    <div class="container">
        <div class="row">
            <div class="col-6">
                <img src="/images/header/acai-logo.svg" alt="Acai Logo" id="logo">
            </div>
            <div class="col-6" id="header-right">
                <div class="left">
                    <img src="/images/header/cart-icon.svg" alt="Cart Icon" id="cart">
                </div>
                <div class="right">
                    <img src="/images/header/menu.svg" alt="Menu" id="burger">
                </div>
            </div>
        </div>
    </div>
</header>