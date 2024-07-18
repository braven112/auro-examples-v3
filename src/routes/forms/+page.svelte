<script context="module">
  export const prerender = true;
</script>

<script>
  import FormExamples from "$lib/content/FormExamples.svelte";
  import FlightSearchForm from "$lib/content/FlightSearchForm.svelte"
</script>

<svelte:head>
  <title>Forms: All of our auro form elements on one page</title>
</svelte:head>

<div class="mainContent">
  <auro-header>Auro Forms</auro-header>
    <p>
      This page is intended to show all of our form elements all on one page. This page is NOT intended to show how we should do things. Its intended to show how they CAN be
      implemented. This way we can align on fallbacks if necessary and find any potential bugs. We'll continue to add more examples.
    </p>
  <div class="row from-bg">
    <auro-header display="700">background</auro-header>
    <FormExamples />
  </div>
  <div class="row defalt">
    <auro-header display="700">No background</auro-header>
    <FormExamples />
  </div> 
  <auro-button onClick="toggleDialog('#demo1')">Open Default Dialog</auro-button>
  <auro-dialog id="demo1">
    <span slot="header">[header content]</span>
    <span slot="content">
      [body content]
    </span>
    <span slot="footer">
      [footer content]
    </span>
  </auro-dialog>
</div>

<style>
  .mainContent {
    padding: var(--padding);
    display: block;
  }
  .row {
    margin-bottom: 3rem;
    padding: var(--padding);
    border: 1px solid var(--auro-color-border-disabled-on-light);
    border-radius: var(--auro-border-radius);
  }
  .from-bg {
    background-color: #eee;
  }
</style>
