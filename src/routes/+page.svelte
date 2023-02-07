<script>
	import FooterTa from '$lib//footer/FooterTA.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	Default page
</section>

<style>
	section {
		display: grid;
		justify-content: space-around;
		margin-top: 2rem;
	}
</style>

