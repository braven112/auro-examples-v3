<script>
  import article from "./Article_Content.json";
  import author from "./Author.json";
</script>
<article class="article" data-variant="1">
  <auro-header margin="bottom" size="none">{article.headline}</auro-header>
  
  <div class="author_socials">
    <span class="article_author">Author: {article.author}</span>
    <span class="author_linkedin"><auro-hyperlink href={author.linkedin_url}><auro-icon category="social" name="linkedin" ariaHidden="false"></auro-icon></auro-hyperlink></span>
    <span class="author_x"><auro-hyperlink href={author.x_url}><auro-icon category="social" name="twitter" ariaHidden="false"></auro-icon></auro-hyperlink></span>
    <span class="author_youtube"><auro-hyperlink href={author.youtube_url}><auro-icon category="social" name="youtube" ariaHidden="false"></auro-icon></auro-hyperlink></span>
    <span class="author_instagram"><auro-hyperlink href={author.instagram_url}><auro-icon category="social" name="instagram" ariaHidden="false"></auro-icon></auro-hyperlink></span>
</div>
  <div class="article_date">Last Updated: {article.lastUpdatedOnDate}</div>
  <span class="article_readminutes"><auro-icon category="interface" name="calendar" ariaHidden="false"></auro-icon> {article.minutes} min. read</span>
  <span class="article_tags"><auro-icon category="interface" name="tag" ariaHidden="false"></auro-icon> <auro-hyperlink href={author.youtube_url}>Bunnies</auro-hyperlink>, <auro-hyperlink href={author.youtube_url}>Badgers</auro-hyperlink>, <auro-hyperlink href={author.youtube_url}>Beavers</auro-hyperlink></span>
  <div class="article_summary">TLDR; {article.summary}</div>
  <div class="article_full">{article.full}</div>
</article>

<style>
  .article {
    padding-bottom: var(--article-gap);
    border-bottom: 1px solid var(--ds-color-border-disabled-default);
  }
  .author_socials {
        display: grid;
        grid-template-columns: max-content min-content min-content min-content min-content;
        gap: var(--ds-size-100);
        align-items: center;
    }
  .article_author,.article_date,.article_readminutes {
    font-size: var(--ds-text-body-size-sm);
    color: var(--auro-color-text-secondary-on-light);
  }
  .article_summary {
    background-color: var(--ds-color-background-lighter);
    padding: var(--article-gap);
    margin-block: var(--article-gap);
    border-left: 8px solid var(--ds-color-background-darker);
    font-size: var(--ds-text-body-size-lg);
  }
</style>