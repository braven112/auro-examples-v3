<script>
  import "./Merch3.css";
  import planes from '$lib/images/planes.svg';
  import lines from '$lib/images/lines.svg';
</script>
<article class="merch" data-variant="3">
  <picture class="merch__img">
    <!-- <img class="imgholder" src={card} alt="Card" /> -->
    <div class="merch__graphics">
      <auro-avatar type="md" code="HNL"></auro-avatar>
      <div class="product__offer-wrapper">
        <div class="product__offer">80K</div>
        <div class="product__offer-detail">+ $6</div>
      </div>
      <img class="product__graphic-detail" src={planes} alt="planes" />
    </div>
  </picture>
  <div class="merch__content">
      <p class="product__title-sm" data-type="headline-sm">Aloha Anita</p>
      <p class="product__title-md" data-type="headline-md">Aloha Anita</p>
      <p class="product__title-lg" data-type="headline-lg">Aloha Anita</p>
      <p class="product__bodycopy" data-type="bodycopy">A flight you just searched is as low as 40K miles + $6 one way</p> 
      <p class="product__flight-details auro_heading auro_heading--300" data-type="flight-details">Seattle, WA <sup class="airport-code">Sea</sup> <auro-icon category="interface" name="arrow-right"></auro-icon> Honolulu, HI <sup class="airport-code">HNL</sup></p> 
      <p class="product__flight-date" data-type="flight-date"><auro-icon category="interface" name="calendar"></auro-icon> Monday, April 1st</p> 
      <auro-hyperlink class="product__cta-sm" data-type="standard" type="nav" href="https://www.alaskaair.com">Explore Now ></auro-hyperlink>   
      <div class="product__graphic-wrapper">
        <img class="product__graphic-lines" src={lines} alt="lines" />
      </div>
  </div>
</article>


<style>

</style>
      