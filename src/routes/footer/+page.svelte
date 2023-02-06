<script context="module">
  export const prerender = true;
</script>

<script>
    import SideNav3ColExample from "$lib/content/SideNav3ColExample.svelte";
    import Footer from "$lib/footer/Footer.svelte";
    import FooterAlt from "$lib/footer/FooterAlt.svelte";
    import MerchFooter from "$lib/footer/MerchFooter.svelte";




 
</script>

<svelte:head>
  <title>Footer: Demo of a Footer</title>
</svelte:head>


<SideNav3ColExample />
<MerchFooter />
<Footer />
<MerchFooter />
<FooterAlt />

