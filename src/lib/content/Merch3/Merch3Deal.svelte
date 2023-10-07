<script>
  import "./Merch3.css";
  import planes from '$lib/images/planes.svg';
  import lines from '$lib/images/lines.svg';
</script>
<article class="merch" data-variant="3">
  <picture class="merch__img">
    <!-- <img class="imgholder" src={card} alt="Card" /> -->
    <div class="merch__graphics">
      <auro-avatar type="md" code="anc"></auro-avatar>
      <div class="product__offer-wrapper">
        <div class="product__offer">$49</div>
        <div class="product__offer-detail">one way</div>
      </div>
      <img class="product__graphic-detail" src={planes} alt="planes" />
    </div>
  </picture>
  <div class="merch__content">
      <p class="product__title-sm" data-type="headline-sm">Hey Anita</p>
      <p class="product__title-md" data-type="headline-md">Hey Anita</p>
      <p class="product__title-lg" data-type="headline-lg">Hey Anita</p>
      <p class="product__bodycopy" data-type="bodycopy">A flight you just searched is as low as $49 one way</p> 
      <p class="product__flight-details auro_heading auro_heading--300" data-type="flight-details">Seattle, WA <sup class="airport-code">Sea</sup> <auro-icon category="interface" name="arrow-right"></auro-icon> Anchorage, AK <sup class="airport-code">ANC</sup></p> 
      <p class="product__flight-date" data-type="flight-date"><auro-icon category="interface" name="calendar"></auro-icon> Monday, April 1st</p> 
      
      <auro-hyperlink class="product__cta-sm" data-type="standard" type="nav" href="https://www.alaskaair.com">Book Now ></auro-hyperlink>
      <auro-hyperlink class="product__cta-md" type="cta" href="https://www.alaskaair.com">Book Now</auro-hyperlink>
      <p class="product__fineprint-xs fineprint">Restrictions apply</p>
      <p class="product__fineprint-sm fineprint">Terms and conditions apply. Must apply here. Offers vary elsewhere.</p>
      <p class="product__fineprint-lg fineprint">Terms and conditions apply. Must apply here. Offers vary elsewhere. Offer void outside of the United States.  Must complete applicaton in English.</p>
      <div class="product__graphic-wrapper">
        <img class="product__graphic-lines" src={lines} alt="lines" />
      </div>
  </div>
</article>


<style>

</style>
      