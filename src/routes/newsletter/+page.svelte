<!-- <script context="module">
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

</style> -->

<script context="module">
  export const prerender = true;
</script>

<script>
  import ArticleSummary from "$lib/content/Article/ArticleSummary.svelte";
  import author from "$lib/content/Article/Author.json";
</script>

<svelte:head>
  <title>Newsletter: Some title of the newsletter</title>
</svelte:head>


<div class="mainContent">
  <div class="articles">
    <div>
    <auro-header margin="both" size="none">Auro Newsletter</auro-header>
    <span class="newsletter_tagline">Your UX and Front End Newsletter</span>
  </div>
    <ArticleSummary></ArticleSummary>
    <ArticleSummary></ArticleSummary>
    <ArticleSummary></ArticleSummary>
  </div>
  <aside>
    <auro-header display="500" margin="both" size="none"><auro-icon category="interface" name="tag" ariaHidden="false"></auro-icon> Tags</auro-header>
    <span class="article_tags"><auro-hyperlink href="https://auro-examples.vercel.app/newsletter">Bunnies</auro-hyperlink>, <auro-hyperlink href="https://auro-examples.vercel.app/newsletter">Badgers</auro-hyperlink>, <auro-hyperlink href="https://auro-examples.vercel.app/newsletter">Beavers</auro-hyperlink></span>
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
    display: grid;
    gap:var(--article-gap);
  }

</style>

