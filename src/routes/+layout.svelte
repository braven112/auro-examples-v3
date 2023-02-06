<script>
	import Header from '$lib/header/Header.svelte'
    import MerchFooter from '$lib/footer/MerchFooter.svelte';
    import FooterAlt2 from '$lib/footer/FooterAlt2.svelte';
	import '../app.css';

  let analyticsId = import.meta.env.VERCEL_ANALYTICS_ID;

</script>

<Header />

<main>
	<slot />
</main>
<MerchFooter />
<FooterAlt2 />

