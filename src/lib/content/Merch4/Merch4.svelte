<script>
  import "./Merch4.css";
  import card from '$lib/images/as-card.svg';
  import campaign from '../personal/Campaign_DataCC.json';
</script>
<div class="merch-container">
<article class="merch" data-variant="4">

  <div class="merch__content">
    <!--Title-->  
    <p class="product__title product__title-sm" data-type="title-sm">{campaign.titleSm}</p>
    <p class="product__title product__title-md" data-type="title-md">{campaign.titleMd}</p>
    <p class="product__title product__title-lg" data-type="title-lg">{campaign.titleLg}</p>  
    <!--Headlines-->  
    <p class="product__headline product__headline-sm" data-type="headline-sm">{campaign.headlineSm}</p>
    <p class="product__headline product__headline-md" data-type="headline-md">{campaign.headlineMd}</p>
    <p class="product__headline product__headline-lg" data-type="headline-lg">{campaign.headlineLg}</p>
    <!--CTA-->
    <auro-hyperlink ondark class="product__cta-md" data-type="standard" type="nav" href="{campaign.ctaLinkMd}?{campaign.campaignId}">{campaign.ctaMd}</auro-hyperlink>
    <!--Disclaimer-->
    <p class="product__fineprint-sm fineprint">{campaign.fineprintSm}</p>
    <p class="product__fineprint-md fineprint">{campaign.fineprintMd}</p>
    <p class="product__fineprint-lg fineprint">{campaign.fineprintLg}</p>
  </div>
  <picture class="merch__img">
      <img class="product__graphic-detail" src={card} alt="card" />
  </picture>
</article>
</div>