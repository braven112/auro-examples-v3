<script>
  import article from "./Article_Content.json";
</script>
<article class="article" data-variant="1">
  <auro-header margin="bottom" size="none">{article.headline}</auro-header>
  <span class="article_author">Author: {article.author} | </span>
  <span class="article_date">Last Updated: {article.lastUpdatedOnDate}</span>
  <div class="article_summary">TLDR; {article.summary}</div>
  <div class="article_full">{article.full}</div>
</article>

<style>
  :root {
    --readable-window: 800px;
  }
.article {
  padding-bottom: var(--article-gap);
  border-bottom: 1px solid var(--ds-color-border-disabled-default);
  max-width: var(--readable-window);
}
  .article_author,.article_date {
    font-size: .8rem;
    color: var(--auro-color-text-secondary-on-light);
  }
  .article_summary {
    background-color: var(--ds-color-background-lighter);
    padding: var(--article-gap);
    margin-block: var(--article-gap);
    border-left: 8px solid var(--ds-color-background-darker);
  }

</style>