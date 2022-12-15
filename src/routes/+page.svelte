<script>
	import './styles.css';

	let links = {
		'1.link': 'https://soundcloud.com/discover',
		'1.label': 'Soundcloud',
		'2.link': 'https://google.com',
		'2.label': 'Google',
		'3.link': 'https://github.com/',
		'3.label': 'Github',
		'4.link': 'https://Youtube.com',
		'4.label': 'Youtube'
	};

</script>

<svelte:head>
	<title>cards</title>
	<meta name="description" content="NewTab page!" />
</svelte:head>

<section>
	<h1>Welcome, Ready to browse the net?</h1>
	<div class="cardContainer">
		<a class="card-link" href="{links['1.link']}">
			<div class="card">
				<img src="logos/{links['1.label']}-logo.png" alt="{links['1.label']}" width="100%" />
				<div class="container subitle" />
			</div>
		</a>
		<a class="card-link" href="{links['2.link']}">
			<div class="card">
				<img src="logos/{links['2.label']}-logo.png" alt="{links['2.label']}" width="100%" />
				<div class="container subitle" />
			</div>
		</a>
		<a class="card-link" href="{links['3.link']}">
			<div class="card">
				<img src="logos/{links['3.label']}-logo.png" alt="{links['3.label']}" width="100%" />
				<div class="container subitle" />
			</div>
		</a>
		<a class="card-link" href="{links['4.link']}">
			<div class="card">
				<img src="logos/{links['4.label']}-logo.png" alt="{links['4.label']}" width="100%" />
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
