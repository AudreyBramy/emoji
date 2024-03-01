<script>
	import { copy } from 'svelte-copy';
</script>

<h2>Ma liste d'emojis clickable</h2>
<ul>
	<li > Pour dire que t'es d'accord <button use:copy={'👍'}>👍</button></li>
	<li > Pour envoyer du réconfort ou du love <button use:copy={'💗 '}>💗 </button></li>
	<li > Saluer <button use:copy={'👏'}>👏</button></li>
	<li > Signaler que tu as bien vu <button use:copy={'👀'}>👀</button></li>
</ul>
<style lang="scss">
	
	:global(main) {
		padding: 4em 20em;
		max-width: 240px;
		margin: 0 auto;

		@media (min-width: 640px) {
			max-width: none;
		}
	}

	button {
		background-color: white;
		border: none;
		font-size: 1.5em;
		padding: 0.5em 0;
	}

	h2 {
		color: #000;
		text-transform: uppercase;
		font-size: 2em;
		font-weight: 100;
	}
	
</style>
