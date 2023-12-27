<script context="module">
  export const prerender = true;
</script>

<script>
  import ArticleSummary from "$lib/content/Article/ArticleSummary.svelte";
</script>

<svelte:head>
  <title>Newsletter: Some title of the newsletter</title>
</svelte:head>


<div class="mainContent">
  <auro-header margin="bottom" size="none">Auro Newsletter</auro-header>
  <span class="newsletter_tagline">Your UX and Front End Newsletter</span>
  <div class="articles">
    <ArticleSummary></ArticleSummary>
    <ArticleSummary></ArticleSummary>
    <ArticleSummary></ArticleSummary>
  </div>
</div>

<style>
  :root {
    --article-gap: var(--ds-size-300);
    --newsletter_tagline: var(--ds-color-brand-breeze-300);
  }
	.mainContent {
    padding: var(--padding);
    display: block;
  }
  .newsletter_tagline {
    color: var(--newsletter_tagline);
  }
  .articles {
    margin-top: calc(2 * var(--article-gap));
    display: grid;
    gap:var(--article-gap);
  }

</style>
