<script>
  import article from "./Article_Content.json";
</script>
<article class="articleSummary" data-variant="1">
  <auro-header display="600" margin="bottom" size="none">{article.headline}</auro-header>
  <span class="articleSummary_author">Author: {article.author} | </span>
  <span class="articleSummary_date">Last Updated: {article.lastUpdatedOnDate}</span>
  <p class="articleSummary_summary">{article.summary} <auro-hyperlink href={article.ctaLink}>{article.cta}</auro-hyperlink></p>
</article>

<style>
.articleSummary {
  padding-bottom: var(--article-gap);
  border-bottom: 1px solid var(--ds-color-border-disabled-default);
}
  .articleSummary_author,.articleSummary_date {
    font-size: .8rem;
    color: var(--auro-color-text-secondary-on-light);
  }

</style>