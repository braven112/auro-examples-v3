<script>
	import Hero from '$lib/content/HeroCC.svelte';
	import Merch3 from '$lib/content/Merch3/Merch3.svelte';
	import Merch3Alert from '$lib/content/Merch3Alert/Merch3Alert.svelte';
	import Merch4 from '$lib/content/Merch4/Merch4.svelte';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<Hero />
</section>
<section>
	<div class="homeContainer">
		<Merch3Alert />
	</div>
</section>
<section>
	<div class="homeContainer">
		<Merch3 />
	</div>
</section>
<section>
	<div class="homeContainer">
		<Merch4 />
	</div>
</section>

<style>
	section {
		margin-bottom: 2rem; 
	}
	.homeContainer {
		max-width: 1232px;
		margin: auto;
		padding: 0 var(--auro-size-xl);
		display: grid;
   		gap: var(--auro-size-sm);
	}
</style>

