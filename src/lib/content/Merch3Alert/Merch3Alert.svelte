<script>
	import lines from '$lib/images/lines.svg';
	import campaign from '../personal/Campaign_Data.json';
	import flight from '../personal/Flight_Data.json';
	import './Merch3Alert.css';
</script>
<div class="merch-container">
  <article class="merchAlert" data-variant="3" style="background-image: url({lines})">
    <picture class="merch__img">
      <div class="merch__graphics">
        <auro-avatar sm type="sm" code={flight.destinationCode} />
      </div>
    </picture>
    <div class="merch__content" >
      <!--Body Copy-->
      <p class="product__bodycopy-sm" data-type="bodycopy"><auro-icon category="terminal" name="plane-side-stroke"></auro-icon> {campaign.bodyCopySm}</p>
      <p class="product__bodycopy-md" data-type="bodycopy"><auro-icon category="terminal" name="plane-side-stroke"></auro-icon> {campaign.bodyCopyMd}</p>
      <p class="product__bodycopy-lg" data-type="bodycopy"><auro-icon category="terminal" name="plane-side-stroke"></auro-icon> {campaign.bodyCopyLg}</p>
      <!--CTA-->
      <auro-hyperlink class="product__cta-md" data-type="standard" type="nav" href="{campaign.ctaLinkMd}?{campaign.campaignId}">{campaign.ctaMd}</auro-hyperlink>
  </article>
</div>
