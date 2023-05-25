<script>
	import { page } from "$app/stores";

    console.log($page.url.pathname)

</script>

<style>
    header {
        background-color: #50253D;
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
    <div class="nav-container">
        <div class="row">
            <div class="col-6">1</div>
            <div class="col-6">2</div>
        </div>
    </div>
</header>


<!--<header>
    <div class="container">
        <div class="row">
            <div class="col-xl-3" id="logo-col">
                <a href="/">
                    <img src="/images/header/acai-logo.svg" alt="Acai Logo" id="acai-logo">
                </a>
            </div>
            <div class="col-xl-6 text-center" id="menu-col">
                <ul class="nav-menu">
                    <a href="/shop" class:active={$page.url.pathname === "/shop"}>
                        <li>SHOP</li>
                    </a>
                    <a href="/about-us" class:active={$page.url.pathname === "/about-us"}>
                        <li>ABOUT US</li>
                    </a>
                    <a href="/stores" class:active={$page.url.pathname === "/stores"}>
                        <li>STORES</li>
                    </a>
                    <a href="/blog" class:active={$page.url.pathname === "/blog"}>
                        <li>BLOG</li>
                    </a>
                </ul>
            </div>
            <div class="col-xl-3" id="account-col">
                <div class="icon-container">
                    <div class="icon-half-1">
                        <img src="/images/header/cart-icon.svg" alt="Cart Icon">
                    </div>
                    <div class="icon-half-2">
                        <img src="/images/header/account.svg" alt="Icon of a person">
                    </div>
                </div>
            </div>
        </div>
    </div>
</header>-->