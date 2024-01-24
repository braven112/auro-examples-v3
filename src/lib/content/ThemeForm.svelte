<script>
  import CityMenuOptions from "$lib/content/CityMenuOptions.svelte";
</script>

<div class="formWrapper">
  <!-- <div class="auro-datetime">Today is <auro-datetime type="date" month="long" weekday="long" /></div>
  <auro-header level="2" margin="top" size="none" display="600">Let's go somewhere!</auro-header> -->
  <auro-combobox >
    <span slot="label">From</span>
    <auro-menu>
      <CityMenuOptions />
    </auro-menu>
  </auro-combobox>
  <auro-combobox >
    <span slot="label">To</span>
    <auro-menu>
      <CityMenuOptions />
    </auro-menu>
  </auro-combobox>
  <auro-datepicker>
    <span slot="fromLabel">Departure</span>
    <span slot="toLabel">Return</span>
    <span slot="mobileDateLabel">Roundtrip</span>
  </auro-datepicker>
  <auro-button fluid>Search</auro-button>
</div>

<style>
  auro-input,
  auro-combobox, auro-datepicker {
    margin-bottom: var(--auro-size-md);
  }
  .formWrapper {
    background-color: var(--ds-color-background-lightest);
    display: flex;
    flex-direction: column;
  }

 
    .formWrapper {
      width: 25rem;
      background-color: var(--ds-color-background-lightest);
      padding: var(--auro-size-xxl) var(--padding);
      border-radius: 0.25rem;
      display: flex;
      flex-direction: column;
      box-shadow: 0 0.25rem 0.75rem rgb(0 0 0 / 10%);
    }
    
</style>
