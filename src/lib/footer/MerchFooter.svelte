<script>
	import Merch3Award from '$lib/content/Merch3/Merch3Award.svelte';
	import Merch3Deal from '$lib/content/Merch3/Merch3Deal.svelte';
import card from '$lib/images/card.png';
</script>
<div class="footer-merch-background">
  <div class="footer-merch-containers">
    <div class="footer-merch-container">
    <Merch3Award />
    </div>
    <div class="footer-merch-container">
    <Merch3Deal />
  </div>
  </div>
</div>

<style>
  .footer-merch-background {
    background: var(--ds-color-background-primary-100-default);
  }
  .footer-merch-containers {
    display: grid;
    gap: var(--auro-size-sm);
    padding: var(--auro-size-xl);
    max-width: 1232px;
    margin: var(--auro-size-xl) auto 0;
  }
  .footer-merch-container {
    container-type: inline-size;
  }
  @media screen and (min-width: 575px) {
    .footer-merch-containers {
      gap: var(--auro-size-sm);
    }
  }

  @media screen and (min-width: 900px) {
    .footer-merch-containers {
      gap: var(--auro-size-md);
      grid-template-areas: 'merch1 merch2';
      grid-template-columns: 1fr 1fr;
    }
  }

  @media screen and (min-width: 1024px) {
    .footer-merch-containers {
      gap: var(--auro-size-lg);
    }
  }

  @media screen and (min-width: 1440px) {
    .footer-merch-containers {
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
