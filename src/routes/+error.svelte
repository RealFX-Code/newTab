<script>
	// @ts-nocheck

	import { page } from '$app/stores';
	import './styles.css';
</script>

<section>
	<div class="alert">
		<h1 id="title">{$page.status}: {$page.error.message}</h1>
		<h2 id="subtitle">I don't know what happened, but something isn't right!</h2>
	</div>
</section>

<style>
	* {
		margin: 0;
		padding: 0;
		text-align: center;
		font-weight: bold;
	}

	div.alert {
		margin: auto;
	}

	div.alert #title {
		font-size: 5em;
	}
	div.alert #subtitle {
		font-size: 2em;
	}
</style>
