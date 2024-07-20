<style>
    .badge-grid {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(16rem, 1fr));
        gap: var(--ds-size-100);
        
    }
</style>
<div class="badge-grid">
    <auro-badge pill>Default</auro-badge>
    <auro-badge pill mvp>MVP</auro-badge>
    <auro-badge pill mvpgold>MVP Gold</auro-badge>
    <auro-badge pill emerald><b>one</b>world Emerald</auro-badge>
    <auro-badge pill sapphire><b>one</b>world Sapphire</auro-badge>
    <auro-badge pill ruby><b>one</b>world Ruby</auro-badge>
    <auro-badge pill lounge>Lounge</auro-badge>
    <auro-badge pill loungeplus>Lounge Plus</auro-badge>
    <auro-badge error pill>Danger</auro-badge>
    <auro-badge success pill>Flight 167</auro-badge>
    <auro-badge advisory pill>99</auro-badge>
    <auro-badge pill style="color: var(--auro-color-text-primary-on-light); background-color: var(--auro-color-brand-tropical-300); border-color: var(--auro-color-brand-tropical-300)">Flight 99</auro-badge>
</div>