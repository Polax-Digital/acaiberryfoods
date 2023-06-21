<style>
    .carousel-container {
        width: 100%;
        display: block;
        overflow: hidden;
    }
    .carousel {
        display: block;
        width: 100%;
        min-height: 525px;
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
        max-width: 300px;
        position: relative;
        min-height: 200px;
        margin-right: 1rem;
    }
    .item > div {
        white-space: normal;
        position: absolute;
        font-family: NowAltRegular;
    }
    .name {
        color: #50253D;
        margin-bottom: 0px;
        font-size: 1.1rem;
    }
    .occ {
        margin-top: 5px;
        margin-bottom: 5px;
        font-size: 0.9rem;
        font-family: NowAltLight;
    }
    .first {
        margin-left: 1rem;
    }
    .last {
        margin-right: 0px;
    }
    .item > div > img {
        height: 410px;
    }
</style>

<div class="carousel-container">
    <div class="carousel">
        <div class="item first">
            <div>
                <p class="name">Caio Castro</p>
                <p class="occ">Brazilian Actor</p>
                <img src="/images/people/caio.png" alt="Caio Castro">
            </div>
        </div>
        <div class="item">
            <div>
                <p class="name">Douglas Costa</p>
                <p class="occ">Brazilian Footballer</p>
                <img src="/images/people/douglas.png" alt="Douglas Costa">
            </div>
        </div>
        <div class="item">
            <div>
                <p class="name">Philippe Coutinho</p>
                <p class="occ">Brazilian Footballer</p>
                <img src="/images/people/philippe.png" alt="Philippe Coutinho">
            </div>
        </div>
        <div class="item last">
            <div>
                <p class="name">Thiago Silva</p>
                <p class="occ">Brazilian Footballer</p>
                <img src="/images/people/thiago.png" alt="Thiago Silva">
            </div>
        </div>
    </div>
</div>