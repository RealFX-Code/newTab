<script>
</script>

<svelte:head>
	<title>About newTab!</title>
	<meta name="description" content="What's it really about?" />
</svelte:head>

<section>
	<div class="about">
		<h1>What is newTab?</h1>
		<div class="text">
			<p>
				This is a new tab page, You can put it as yours if you'd like.
				I just have my most used websites pinned to the front page, if you host it yourself, you can use your own link.
			</p>
			<p>
				Contributor? &RightArrow; <a href="https://github.com/RealFX-Code/newtab">Check out the github page!</a>
			</p>
		</div>
	</div>
</section>

<style>
	h1 {
		font-size: 3rem;
		font-weight: bolder;
	}
	div.text {
		margin: auto;
		word-wrap: normal;
		line-break: strict;
		width: 75vw;
	}
	@media only screen and (max-width: 600px) {
		div.text {
			width: 100%;
		}
	}
	p {
		font-size: 2rem;
	}
</style>
