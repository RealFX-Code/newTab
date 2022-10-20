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
			<p>newTab is my new tab bage for my web brosers. Kinda obvious really...
				You've got four cards on the main page, where you click them and they take you to wherever they say they will.
				And these tabs that you've found, They contain other stuff that I may find useful at any time.</p>
			<p>If you have anything you'd like to say about this, or make a feature, or fix something, send me an issue or pull request at the
				<a href="https://github.com/RealFX-Code/newtab">Github</a>
				page.</p>
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
