<script>
	import { spring } from 'svelte/motion';
</script>

<div class="glowna">
	<h1>
		To jest strona o przepisach
	</h1>
	<p>
		Strona "Counter.svelte" jest częścią aplikacji SvelteKit.
		 Zawiera prosty licznik, który można zwiększać i zmniejszać za pomocą 
		 przycisków. Wygląd strony jest zdefiniowany za pomocą styli CSS, które 
		 nadają elementom odpowiednie właściwości i wygląd.
	</p>
	
</div>

<style>
	.glowna {
		display: flex;
		border-top: 1px solid rgba(0, 0, 0, 0.1);
		border-bottom: 1px solid rgba(0, 0, 0, 0.1);
		margin: 1rem 0;
	}

	button {
		width: 2em;
		padding: 0;
		display: flex;
		align-items: center;
		justify-content: center;
		border: 0;
		background-color: transparent;
		touch-action: manipulation;
		font-size: 2rem;
	}

	.counter button:hover {
		background-color: var(--color-bg-1);
	}

	svg {
		width: 25%;
		height: 25%;
	}

	path {
		vector-effect: non-scaling-stroke;
		stroke-width: 2px;
		stroke: #444;
	}
</style>
