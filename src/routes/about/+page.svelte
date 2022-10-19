<script>
	// wow, me making future plans for multiple languages??

	let lang = {
		hero: 'What is newTab?',
		para1_1: 'newTab is my start tab, mostly just for me to write something.',
		para1_2: "Don't expect alot.",
		para2_1: 'If you want to know more,',
		para2_2: 'Check the project out on '
	};
</script>

<svelte:head>
	<title>About newTab!</title>
	<meta name="description" content="What's it really about?" />
</svelte:head>

<section>
	<div class="about route">
		<h1>{lang.hero}</h1>
		<section class="section one">
			<p>{lang.para1_1}</p>
			<p>{lang.para1_2}</p>
		</section>
		<section class="section two">
			<p>{lang.para2_1}</p>
			<p>
				{lang.para2_2}
				<a href="https://github.com/RealFX-Code/newTab">GitHub</a>
			</p>
		</section>
	</div>
</section>

<style>
	div.about h1 {
		font-size: 10rem;
		font-weight: bolder;
	}
	div.about p {
		font-size: 3rem;
		font-weight: bold;
	}
</style>
