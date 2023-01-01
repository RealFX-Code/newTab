<script>
	import './styles.css';

	const links = [
		{
			link: "https://soundcloud.com/",
			label: "Soundcloud"
		},
		{
			link: "https://google.com/",
			label: "Google"
		},
		{
			link: "https://github.com/",
			label: "Github"
		},
		{
			link: "https://youtube.com/",
			label: "Youtube"
		}
	]

</script>

<svelte:head>
	<title>cards</title>
	<meta name="description" content="NewTab page!" />
</svelte:head>

<section>
	<h1>NewTab - Some links, or whatever</h1>
	<div class="cardContainer">
		{#each links as { link, label }}
			<a class="card-link" href="{link}">
				<div class="card">
					<img src="logos/{label}-logo.png" alt="{label}" width="100%" />
				</div>
			</a>
		{/each}
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
