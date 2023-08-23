<script>
    let title = "6x Acai Berry Tubs - 200ml";
    let price = 23.94;
    let imgurl = "/images/home/berry-tub.png";
    let multiplier = "6x";
</script>
<style>
    .product-container {
        border-radius: 10px;
        background: #fff;
        box-shadow: 0px 0px 15px 0px rgba(0, 0, 0, 0.15);
        padding: 50px;
        max-width: 380px;
    }
    .title {
        color: #000;
        font-family: "Now Alt";
        font-size: 20px;
        font-style: normal;
        font-weight: 700;
        line-height: normal;
        margin: 0;
    }
    .price {
        color: #000;
        font-family: "Now Alt";
        font-size: 20px;
        font-style: normal;
        font-weight: 400;
        line-height: normal;
        margin-top: 10px;
    }
    .img-container {
        margin: 4.5rem 0;
    }
    .prod-img-container {
        text-align: center;
    }
    .multi-container {
        position: relative;
        text-align: left;
        margin-top: -6rem;
        margin-left: 2rem;
    }
    .multiplier-num {
        font-family: "Now Alt";
        font-size: 28px;
        font-weight: 800;
        color: #fff;
        position: absolute;
        top: 50%;
        left: 14%;
        transform: translate(-50%, -50%);
        margin: 0;
    }
    .cart-btn {
        border-radius: 70px;
        border: 3px solid #3C9E36;
        background: #FFF;
        color: #3C9E36;
        font-family: "Now Alt";
        font-size: 13px;
        font-style: normal;
        font-weight: 700;
        line-height: normal;
        margin-bottom: 1.5rem;
    }
    .buy-btn {
        border-radius: 70px;
        border: 3px solid #1B6E16;
        background: #3C9E36;
        color: #fff;
        font-size: 13px;
        font-style: normal;
        font-weight: 700;
        line-height: normal;
    }
    button {
        padding: 1rem;
        width: 100%;
        text-transform: uppercase;
    }
</style>

<div class="product-container">
    <h4 class="title">{title}</h4>
    <p class="price">£{price}</p>
    <div class="img-container">
        <div class="prod-img-container">
            <img src="{imgurl}" alt="Product" class="product-img" />
        </div>
        <div class="multi-container">
            <img src="/images/home/product-multiplier.png" alt="" class="multiplier">
            <p class="multiplier-num">{multiplier}</p>
        </div>
    </div>
    <button class="cart-btn">Add to Cart</button>
    <button class="buy-btn">Buy Now</button>
</div>