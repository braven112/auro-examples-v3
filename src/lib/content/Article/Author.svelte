<script>
    import author from "./Author.json";
    import author_image from '$lib/images/as-card.svg';
  </script>
  <article class="author" data-variant="1">
    <picture>
        <!-- <img class="author_image" src={author_image} alt={author.author} /> -->
        <auro-avatar img="https://picsum.photos/200?random=0"></auro-avatar>
    </picture>
    <auro-header display="600" margin="bottom" size="none">{author.author}</auro-header>
    
    <div class="author_socials">
        <span class="author_linkedin"><auro-icon category="social" name="linkedin" ariaHidden="false"></auro-icon> {author.linkedin} </span>
        <span class="author_x"><auro-icon category="social" name="twitter" ariaHidden="false"></auro-icon> {author.x} </span>
        <span class="author_youtube"><auro-icon category="social" name="youtube" ariaHidden="false"></auro-icon> {author.youtube} </span>
        <span class="author_instagram"><auro-icon category="social" name="instagram" ariaHidden="false"></auro-icon> {author.instagram} </span>
    </div>
    <auro-header display="300" margin="bottom" size="none">About the author</auro-header>
    <p class="author_summary">{author.authorSummary}</p>
  </article>
  
  <style>
    .author_socials {
        display: grid;
        grid-template-columns: auto auto;
    }
    .author_socials > span {
        display: grid;
        font-size: var(--ds-text-body-size-xs);
    }
    .author_summary {
        font-size: var(--ds-text-body-size-sm);
    }
  /* .articleSummary {
    padding-bottom: var(--article-gap);
    border-bottom: 1px solid var(--ds-color-border-disabled-default);
  }
    .articleSummary_author,.articleSummary_date {
      font-size: .8rem;
      color: var(--auro-color-text-secondary-on-light);
    } */
  
  </style>