<script>
	import Modal from './Modal.svelte';

	let showModal = false;
</script>
<style>
    .header {
        color: #fff;
        text-align: center;
        padding: 5rem;
        background-image: url("images/stores/header.png");
        background-size: cover;
        background-position: center;
    }
    .header h1 {
        font-size: 35px;
        font-family: "Now Alt";
        font-weight: 900;
        letter-spacing: 3.5px;
        text-transform: uppercase;
    }
    .header p {
        font-size: 20px;
        font-family: "Now Alt";
        line-height: 50px;
        max-width: 60%;
        margin: 0 auto;
    }
    .page-content {
        width: 85%;
        margin: 0 auto;
        margin-bottom: 5rem;
        padding-top: 4rem;
    }
    .page-content h2 {
        color: #50253D;
        font-size: 29px;
        font-family: "Now Alt";
        font-weight: 600;
        text-transform: uppercase;
        margin: 0;
        margin-bottom: 13px;
    }
    .page-content p {
        font-size: 20px;
        font-family: "Now Alt";
        line-height: 34px;
        margin: 0;
    }
    .page-content img {
        width: 100%;
        margin-bottom: 4.5rem;
    }
    .page-content small {
        color: #3C9E36;
        font-size: 10px;
        font-family: "Now Alt";
        font-weight: 500;
        text-transform: uppercase;
    }
    .hours-btn {
        text-transform: uppercase;
        font-size: 15px;
        font-family: "Now Alt";
        font-weight: 700;
        color: #fff;
        background-color: #3C9E36;
        border: 2px solid #1B6E16;
        border-radius: 70px;
        padding: 1.5rem 3.5rem;
        margin: 3rem 0;
    }
    .hours-btn:hover {
        cursor: pointer;
    }
    #rennovation {
        margin-bottom: 0;
    }
    /* Media Queries */
    @media screen and (max-width: 430px) {
        .header {
            padding: 3rem;
        }
        .header h1 {
            font-size: 15px;
            letter-spacing: 1.5px;
        }
        .header p {
            font-size: 11px;
            line-height: 23px;
            max-width: 100%;
        }
        .page-content h2 {
            margin: 0;
        }
        .page-content img {
            margin-bottom: 1rem;
        }
        .hours-btn {
            margin-top: 1rem;
        }
    }
</style>

<div class="header">
    <h1>Find a Store Near You</h1>
    <p>Perfect for breakfast, lunch or dinner. Made to enjoy in our tropical rainforest-themed stores or delivered straight to your door.</p>
</div>
<div class="page-content">
    <div class="row">
        <div class="col-md-4">
            <img src="images/stores/boxpark.png" alt="BOXPARK Shoreditch Store">
            <h2>Boxpark Shoreditch</h2>
            <p>Box 32,</p>
            <p>2-10 Bethnal Green Road,</p>
            <p>London</p>
            <p>E1 6GY</p>
            <p>TEL: 020 3385 330</p>
            <button class="hours-btn" on:click={() => (showModal = true)}>Opening Hours</button>
        </div>
        <div class="col-md-4">
            <img src="images/stores/carnaby.png" alt="Carnaby Street Store">
            <h2>Carnaby Street</h2>
            <p>G11 Kingly Court,</p>
            <p>Kingly Street,</p>
            <p>London</p>
            <p>W1B 5PW</p>
            <p>TEL: 020 3385 330</p>
            <button class="hours-btn" on:click={() => (showModal = true)}>Opening Hours</button>
        </div>
        <div class="col-md-4">
            <img src="images/stores/chelsea.png" alt="Chelsea Store">
            <h2>Chelsea</h2>
            <p>247</p>
            <p>King's Road,</p>
            <p>London</p>
            <p>SW3 5EL</p>
            <p>TEL: 020 3385 330</p>
            <button class="hours-btn" on:click={() => (showModal = true)}>Opening Hours</button>
        </div>
    </div>
    <div class="row">
        <div class="col-md-4">
            <img src="images/stores/euston.png" alt="Euston Road Store">
            <h2>Euston Road</h2>
            <p>Unit 4,</p>
            <p>338 Euston Road,</p>
            <p>London</p>
            <p>NW1 3AX</p>
            <p>TEL: 020 3385 330</p>
            <button class="hours-btn" on:click={() => (showModal = true)}>Opening Hours</button>
        </div>
        <div class="col-md-4">
            <img src="images/stores/wardour.png" alt="Wardour Street Store">
            <h2>Wardour Street</h2>
            <p>130</p>
            <p>Wardour Street,</p>
            <p>London</p>
            <p>W1F 8ZN</p>
            <p>TEL: 020 3385 330</p>
            <button class="hours-btn" on:click={() => (showModal = true)}>Opening Hours</button>
        </div>
        <div class="col-md-4">
            <img src="images/stores/nottinghill.png" alt="Notting Hill Store">
            <h2 id="rennovation">Notting Hill</h2>
            <small>*Under Rennovation</small>
            <p>196 Kensington Park Road</p>
            <p>Notting Hill,</p>
            <p>London</p>
            <p>W11 2ES</p>
            <p>TEL: 020 3385 330</p>
            <button class="hours-btn" on:click={() => (showModal = true)}>Opening Hours</button>
        </div>
    </div>
</div>

<Modal bind:showModal></Modal>