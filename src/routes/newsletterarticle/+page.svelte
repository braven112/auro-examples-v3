<script context="module">
  export const prerender = true;
</script>

<script>
  import Article from "$lib/content/Article/Article.svelte";
</script>

<svelte:head>
  <title>Newsletter: Some title of the newsletter</title>
</svelte:head>


<div class="mainContent">
    <Article></Article>
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
