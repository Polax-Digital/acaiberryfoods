<script>
	export let showModal; // boolean

	let dialog; // HTMLDialogElement

	$: if (dialog && showModal) dialog.showModal();

    let days = ["Monday", "Tueday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"];
</script>

<!-- svelte-ignore a11y-click-events-have-key-events -->
<dialog
	bind:this={dialog}
	on:close={() => (showModal = false)}
	on:click|self={() => dialog.close()}
>
	<div class="modal-content" on:click|stopPropagation>
		<h3>Open Hours:</h3>
		{#each days as day}
        {#if day == "Sunday"}
            <div class="row">
                <div class="col">
                    <p>{day}</p>
                </div>
                <div class="col">
                    <p>9:00AM - 7PM</p>
                </div>
            </div>
        {:else}
        <div class="row">
            <div class="col">
                <p>{day}</p>
            </div>
            <div class="col">
                <p>7:30AM - 8PM</p>
            </div>
        </div>
        {/if}
      {/each}
      <div class="btn-container">
        <button autofocus on:click={() => dialog.close()} id="close">Close</button>
      </div>
	</div>
</dialog>

<style>
    h3 {
        text-align: center;
        margin: 0;
    }
    p {
        margin: 0;
    }
    #close {
        text-transform: uppercase;
        font-size: 13px;
        font-family: "Now Alt";
        font-weight: 700;
        color: #3C9E36;
        background-color: #fff;
        border: 2px solid #1B6E16;
        border-radius: 70px;
        padding: 1rem 3.5rem;
        margin: 10px auto;
    }
    #close:hover {
        cursor: pointer;
    }
	dialog {
		background-color: #fff;
        margin: auto;
        padding: 0.5rem 1.5rem;
        width: 355px;
        color: #000;
        font-size: 20px;
        font-family: "Now Alt";
        line-height: 45px;
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