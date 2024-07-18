<script>
	import BreadcrumbExample from '$lib/content/BreadcrumbExample.svelte';
	import Hero from '$lib/content/HeroCC.svelte';
	import Merch3 from '$lib/content/Merch3/Merch3.svelte';
	import Merch3Alert from '$lib/content/Merch3Alert/Merch3Alert.svelte';
	import Merch4 from '$lib/content/Merch4/Merch4.svelte';
	import UpcomingTrips from '$lib/content/UpcomingTrips.svelte';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>
<section>
	<div class="homeContainer">
		<BreadcrumbExample />
	</div>
</section>
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
<section>
	<div class="homeContainer">
		<UpcomingTrips />
	</div>
</section>


<style>
	section {
		margin-block: 2rem; 
	}
	.homeContainer {
		max-width: 1232px;
		margin: auto;
		padding: 0 var(--ds-size-400);
		display: grid;
   		gap: var(--ds-size-150);
	}
</style>

