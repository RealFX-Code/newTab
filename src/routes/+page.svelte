<script>
	import './styles.css';
</script>

<svelte:head>
	<title>cards</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<h1>Welcome, Ready to browse the net?</h1>
	<div class="cardContainer">
		<a class="card-link" href="https://soundcloud.com/discover">
			<div class="card">
				<img src="logos/Soundcloud-logo.png" alt="Soundcloud" width="100%" />
				<div class="container subitle" />
			</div>
		</a>
		<a class="card-link" href="https://google.com">
			<div class="card">
				<img src="logos/Google-logo.png" alt="Google" width="100%" />
				<div class="container subitle" />
			</div>
		</a>
		<a class="card-link" href="https://github.com/RealFX-Code/">
			<div class="card">
				<img src="logos/Github-logo.png" alt="Github" width="100%" />
				<div class="container subitle" />
			</div>
		</a>
		<a class="card-link" href="/dev">
			<div class="card">
				<img src="logos/Dev-logo.png" alt="Dev" width="100%" />
				<div class="container subitle" />
			</div>
		</a>
	</div>
</section>

<style>
	section {
		flex-direction: column;
		display: flex;
		justify-content: center;
		align-items: center;
	}

	h1 {
		width: 100%;
	}

	.card-link {
		display: grid;
		align-items: center;
		justify-self: center;
		width: 25vw;
		box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
		transition: 0.3s;
		border-radius: 1rem;
	}

	.card-link:hover {
		box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
	}

	.container {
		padding: 2px 16px;
	}

	.cardContainer {
		padding: 0;
		margin: auto;
		display: grid;
		grid-template-columns: repeat(2, 35vw);
		grid-template-rows: repeat(2, 35vh);
		grid-column-gap: 2vw;
		grid-row-gap: 2vw;
	}
</style>
