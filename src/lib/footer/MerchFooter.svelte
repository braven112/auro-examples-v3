<script>
	import card from '$lib/images/card.png';
</script>
<div class="footer-merch-background">
  <div class="footer-merch-container">
    <div class="merch">
      <img class="imgholder" src={card} alt="Card" />
      <div class="content">
        <auro-header class="leadin" level="3" margin="both" size="none" display="300">Limited time offer</auro-header>
        <auro-header class="mainoffer" level="3" margin="top" size="none" display="500">50,000 bonus miles</auro-header>
        <auro-hyperlink nav href="https://www.alaskaair.com">Learn more</auro-hyperlink>
      </div>
    </div>
    <div class="merch">
      <auro-avatar lg code="FLL"></auro-avatar>
      <div class="content">
        <auro-header class="leadin" level="3" margin="both" size="none" display="300">Insert catchy lead in copy here</auro-header>
        <auro-header class="mainoffer" level="3" margin="top" size="none" display="500">Something impactful</auro-header>
        <auro-hyperlink nav href="https://www.alaskaair.com">Buy the thing</auro-hyperlink>
      </div>
    </div>
  </div>
</div>

<style>
  .footer-merch-background {
    background: var(--auro-color-background-lighter);
  }
  .footer-merch-container {
    display: grid;
    gap: var(--auro-size-sm);
    padding: var(--auro-size-xl);
    max-width: 1232px;
    margin: var(--auro-size-xl) auto 0;
  }
  @media screen and (min-width: 575px) {
    .footer-merch-container {
      gap: var(--auro-size-sm);
    }
  }

  @media screen and (min-width: 900px) {
    .footer-merch-container {
      gap: var(--auro-size-md);
      grid-template-areas: 'merch1 merch2';
      grid-template-columns: 1fr 1fr;
    }
  }

  @media screen and (min-width: 1024px) {
    .footer-merch-container {
      gap: var(--auro-size-lg);
    }
  }

  @media screen and (min-width: 1440px) {
    .footer-merch-container {
      gap: var(--auro-size-xl);
    }
  }
  .merch {
    background: var(--auro-color-base-white);
    border-radius: var(--auro-size-xs);
    box-shadow: var(--auro-elevation-100);
    padding: var(--auro-size-lg);
    display: grid;
    gap: var(--auro-size-lg);
    grid-template-areas: 
    'card'
    'text';
    align-items: center;
  }
  @media screen and (min-width: 475px) {
    .merch {
    background: var(--auro-color-base-white);
    border-radius: var(--auro-size-xs);
    box-shadow: var(--auro-elevation-100);
    padding: var(--auro-size-lg);
    display: grid;
    gap: var(--auro-size-lg);
    grid-template-areas: 'card text';
    grid-template-columns: min-content auto;
    align-items: center;
  }
  }
  .leadin {
    color: var(--auro-color-brand-midnight-500);
  }
  .mainoffer {
    color: var(--auro-color-brand-breeze-400);
  }
  .imgholder {
    width: max-content;
  }
</style>
