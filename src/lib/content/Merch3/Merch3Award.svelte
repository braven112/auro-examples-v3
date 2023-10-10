<script>
  import "./Merch3.css";
  import planes from '$lib/images/planes.svg';
  import lines from '$lib/images/lines.svg';
  import campaign from './Campaign_Data2.json';
  import flight from './Flight_Data2.json';
</script>
<article class="merch" data-variant="3">
  <picture class="merch__img">
    <div class="merch__graphics">
      <auro-avatar type="md" code="{flight.destinationCode}"></auro-avatar>
      <div class="product__offer-wrapper">
        <!-- Offer -->
        <div class="product__offer">{flight.offer}</div>
        <div class="product__offer-detail">{flight.offerDetail}</div>
      </div>
      <!--Design Element-->
      <img class="product__graphic-detail" src={planes} alt="planes" />
    </div>
  </picture>
  <div class="merch__content">
      <!--Headlines-->  
      <p class="product__title-md" data-type="headline-md">{campaign.headlineMd}</p>
      <!--Body Copy-->
      <p class="product__bodycopy" data-type="bodycopy">{campaign.bodyCopyMd}</p> 
      <p class="product__flight-details auro_heading auro_heading--300" data-type="flight-details">{flight.origin} <sup class="airport-code">{flight.originCode}</sup> <auro-icon category="interface" name="arrow-right"></auro-icon> {flight.destination} <sup class="airport-code">{flight.destinationCode}</sup></p> 
      <p class="product__flight-date" data-type="flight-date"><auro-icon category="interface" name="calendar"></auro-icon> Monday, April 1st</p> 
      <!--CTA-->
      <auro-hyperlink class="product__cta-md" data-type="standard" type="nav" href="{campaign.ctaLinkMd}?{campaign.campaignId}">{campaign.ctaMd}</auro-hyperlink>
      <!--Disclaimer-->
      <p class="product__fineprint-sm fineprint">{campaign.fineprintSm}</p>
      <p class="product__fineprint-md fineprint">{campaign.fineprintMd}</p>
      <p class="product__fineprint-lg fineprint">{campaign.fineprintLg}</p>
      <!--Design Element-->
      <div class="product__graphic-wrapper">
        <img class="product__graphic-lines" src={lines} alt="lines" />
      </div>
  </div>
</article>
      