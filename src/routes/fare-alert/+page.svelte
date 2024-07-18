<script context="module">
  export const prerender = true;
</script>

<script>
  import FareAlert from "$lib/content/FareAlert.svelte";
  
</script>

<svelte:head>
  <title>Fare Alert</title>
</svelte:head>

<div class="mainContent">
  <auro-header>Fare Alert</auro-header>
    <p>
      This page is intended to show all of our form elements all on one page. This page is NOT intended to show how we should do things. Its intended to show how they CAN be
      implemented. This way we can align on fallbacks if necessary and find any potential bugs. We'll continue to add more examples.
    </p>
  <div class="row">
    <FareAlert />
  </div>
 
</div>

<style>
  .mainContent {
    padding: var(--padding);
    display: block;
  }
</style>
