<script>
  import "./PriceDrop.css";
  import planes from '$lib/images/planes.svg';
  import lines from '$lib/images/lines.svg';
  import pricedrop from './PriceDrop_Data.json';
  // import flight from './PriceDrop_Data.json';
</script>
<div class="containment">
  <article class="merch" data-variant="3">
    <picture class="merch__img">
      <div class="merch__graphics">
        <auro-avatar type="md" code="{pricedrop.pricedrop_destination}"></auro-avatar>
        <div class="product__offer-wrapper">
          <!-- Offer -->
          <div class="product__offer">{pricedrop.pricedrop_pricedrop_percentage}</div>
          <!-- <div class="product__offer-detail">{pricedrop.pricedrop_flight_type}</div> -->
        </div>
        <!--Design Element-->
        <img class="product__graphic-detail" src={planes} alt="planes" />
      </div>
    </picture>
    <div class="merch__content">
        <!--Headlines-->  
        <p class="product__title" data-type="headline-sm">{pricedrop.headline_small} {pricedrop.pricedrop_first_name}</p>
        <p class="product__title" data-type="headline-md">{pricedrop.headline_medium} {pricedrop.pricedrop_first_name}</p>
        <p class="product__title" data-type="headline-lg">{pricedrop.headline_large} {pricedrop.pricedrop_first_name}</p>
        <!--Body Copy-->
        <p class="product__bodycopy" data-type="bodycopy-sm">{pricedrop.body_copy_small}</p> 
        <p class="product__bodycopy" data-type="bodycopy-md">{pricedrop.body_copy_medium}</p> 
        <p class="product__bodycopy" data-type="bodycopy-lg">{pricedrop.body_copy_large}</p> 
        <p class="product__flight-details auro_heading auro_heading--300" data-type="flight-details">
          {pricedrop.pricedrop_origin_city} 
          <sup class="airport-code">{pricedrop.pricedrop_origin}</sup> 
          <auro-icon category="interface" name="arrow-right"></auro-icon> 
          {pricedrop.pricedrop_destination_city} 
          <sup class="airport-code">{pricedrop.pricedrop_destination}</sup>
        </p> 
        <p class="product__flight-date" data-type="flight-date"><auro-icon category="interface" name="calendar"></auro-icon> 
          {pricedrop.pricedrop_departure_date}
        </p> 
        <!--CTA-->
        <auro-hyperlink class="product__cta-md" data-type="standard" type="nav" href="{pricedrop.cta_medium}?{pricedrop.campaign_id}">{pricedrop.cta_medium}</auro-hyperlink>
        <!--Disclaimer-->
        <p class="product__fineprint-sm fineprint">{pricedrop.fineprint_small}</p>
        <p class="product__fineprint-md fineprint">{pricedrop.fineprint_medium}</p>
        <p class="product__fineprint-lg fineprint">{pricedrop.fineprint_large}</p>
        <!--Design Element-->
        <!-- <div class="product__graphic-wrapper">
          <img class="product__graphic-lines" src={lines} alt="lines" />
        </div> -->
    </div>
  </article>
</div>


