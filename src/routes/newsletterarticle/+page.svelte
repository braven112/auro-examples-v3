<script context="module">
  export const prerender = true;
</script>

<script>
  import Article from "$lib/content/Article/Article.svelte";
	import Author from "$lib/content/Article/Author.svelte";
</script>

<svelte:head>
  <title>Newsletter: Some title of the newsletter</title>
</svelte:head>


<div class="mainContent">
  <div class="articleContainer">
    <Article></Article>
  </div>
  <aside>
    <Author></Author>
  </aside>
</div>

<style>
  :root {
    --page-gap: var(--ds-size-500);
    --article-gap: var(--ds-size-300);
    --newsletter_tagline: var(--ds-color-brand-breeze-300);
  }
	.mainContent {
    padding: var(--padding);
    padding-top: 4rem;
    display: grid;
    gap:var(--page-gap);
  }
  @media screen and (min-width: 768px) {
    .mainContent {
      grid-template-columns: auto 168px;
    }
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
