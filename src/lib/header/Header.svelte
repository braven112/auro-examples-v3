<script>
	import { page } from "$app/stores";
  </script>
  
  <header>
	<div class="container">
	  <div class="header-grid">
		<auro-lockup>
		  <span slot="title">Auro</span>
		  <span slot="subtitle">Examples</span>
		</auro-lockup>
		<nav>
		  <auro-dropdown id="common" aria-label="Label content for screen reader">
			<div class="infobar">
			  <div>
				<div class="infobaritem"><auro-header level="4" margin="both" size="none" display="300">Examples</auro-header></div>
				<div class="infobaritem">
				  <auro-hyperlink href="https://auro-examples.vercel.app/grid">Grid</auro-hyperlink>
				</div>
				<div class="infobaritem">
				  <auro-hyperlink href="https://auro-examples.vercel.app/sidenav">Sidenav</auro-hyperlink>
				</div>
				<div class="infobaritem">
				  <auro-hyperlink href="https://auro-examples.vercel.app/sidenav3col">Sidenav - 3 column</auro-hyperlink>
				</div>
				<div class="infobaritem">
				  <auro-hyperlink href="https://auro-examples.vercel.app/forms">Forms</auro-hyperlink>
				</div>
			  </div>
			</div>
			<auro-icon category="interface" name="navigation-menu" slot="trigger" tabindex="0" />
		  </auro-dropdown>
		</nav>
	  </div>
	</div>
  </header>
  
  <style>
	@media screen and (max-width: 320px) {
		auro-lockup {
			font-size: 10px;
			max-width: 200px;
		}
	}
	.infobar {
	  flex: 1;
	  align-self: center;
	  display: flex;
	  justify-content: space-between;
	  padding: var(--padding);
	}
	.infobar + .infobar {
	  padding-top: 0;
	}
	.infobar > div {
	  display: flex;
	  flex-direction: column;
	}
	.infobaritem {
	  padding: 0 var(--auro-size-md) 0 0;
	}
  
	header {
	  box-shadow: 0 0.25rem 0.75rem rgb(0 0 0 / 10%);
	}
	@media screen and (min-width: 1024px) {
	  nav {
		align-self: center;
		flex-grow: 10;
		justify-content: flex-end;
		display: flex;
	  }
	}
	auro-dropdown#common {
	  padding-left: var(--padding);
	}
	auro-hyperlink span {
	  line-height: 1.75rem;
	  margin-left: 0.5rem;
	}

	.container {
	  display: block;
	  max-width: 1232px;
	  margin: auto;
	  padding: var(--padding);
	}
	.header-grid {
		display: grid;
		grid-template-columns: auto min-content;
	}
  </style>
  