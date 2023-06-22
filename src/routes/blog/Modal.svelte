<script>
	export let showModal1, showModal2, showModal3, showModal4, showModal5; // boolean

	let dialog; // HTMLDialogElement

	$: if (dialog && showModal1) dialog.showModal();
    $: if (dialog && showModal2) dialog.showModal();
    $: if (dialog && showModal3) dialog.showModal();
    $: if (dialog && showModal4) dialog.showModal();
    $: if (dialog && showModal5) dialog.showModal();
</script>

<!-- svelte-ignore a11y-click-events-have-key-events -->
<dialog
	bind:this={dialog}
	on:close={() => (showModal1 = false, showModal2 = false, showModal3 = false, showModal4 = false, showModal5 = false)}
	on:click|self={() => dialog.close()}
>
	<div class="modal-content" on:click|stopPropagation>
        <div class="btn-container">
            <button autofocus on:click={() => dialog.close()} id="close">&#x2715</button>
          </div>
		<slot />
	</div>
</dialog>

<style>
    #close {
        background-color: #F9F2F6;
        border: none;
        border-radius: 50%;
        right: -95%;
        position: relative;
        height: 50px;
        width: 50px;
        font-size: 25px;
    }
    #close:hover {
        cursor: pointer;
    }
	dialog {
		background-color: #fff;
        margin: auto;
        width: 80%;
        padding: 2rem 2rem;
        color: #000;
        border: none;
	}
	dialog::backdrop {
		background: rgba(0, 0, 0, 0.3);
	}
	dialog > div {
		padding: 1em;
	}
	dialog[open] {
		animation: zoom 0.3s cubic-bezier(0.34, 1.56, 0.64, 1);
	}
	@keyframes zoom {
		from {
			transform: scale(0.95);
		}
		to {
			transform: scale(1);
		}
	}
	dialog[open]::backdrop {
		animation: fade 0.2s ease-out;
	}
	@keyframes fade {
		from {
			opacity: 0;
		}
		to {
			opacity: 1;
		}
	}
	button {
		display: block;
	}
</style>