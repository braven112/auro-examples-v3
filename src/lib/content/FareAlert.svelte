<script>
  import CityMenuOptions from "$lib/content/CityMenuOptions.svelte";
</script>

    <div class="formWrapper">
     <auro-header>Set Fare Alert</auro-header>
      <auro-combobox >
        <span slot="label">From</span>
        <span slot="helpText">Please enter your departure city</span>
        <auro-menu>
          <CityMenuOptions />
        </auro-menu>
        
      </auro-combobox>
      <auro-combobox >
        <span slot="label">To</span>
        <span slot="helpText">Please enter your destination city</span>
        <auro-menu>
          <CityMenuOptions />
        </auro-menu>
      </auro-combobox>
      <auro-input value="$199" bordered>
        <span slot="label">Max Price</span>
        <span slot="helptext">Please enter your max price</span>
      </auro-input>
      <auro-datepicker range>
        <span slot="fromLabel">Departure</span>
        <span slot="toLabel">Return</span>
        <span slot="mobileDateLabel">Roundtrip</span>
        <span slot="helpText">Please enter your dates</span>
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
      width: 35rem;
      background-color: var(--ds-color-background-lightest);
      padding: var(--auro-size-xxl) var(--padding);
      border-radius: 0.25rem;
      display: flex;
      flex-direction: column;
      box-shadow: 0 0.25rem 0.75rem rgb(0 0 0 / 10%);
    }
    
</style>
