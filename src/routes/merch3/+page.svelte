<script context="module">
	export const prerender = true;
</script>

<script>
	import Merch3Alert from '$lib/content/Merch3Alert/Merch3Alert.svelte'
	import Merch3AlertDeal from '$lib/content/Merch3Alert/Merch3AlertDeal.svelte';
</script>

<svelte:head>
	<title>Merch: Demo of some of the ways to layout merchandising</title>
</svelte:head>

<div class="mainContent">
    
	<auro-header level="2" display="800">Merch Alert Component</auro-header>
	<p>The Deal Alert Component is intended to be a single line alert showing either a price drop, flight deal or an award sale.  Its intended to be used in a full width page or in the main column of a page on mobile or desktop.</p>
	<auro-header level="3" display="600">Price Drop</auro-header>
  <auro-header level="2" display="400">Full width</auro-header>
	<div class="container"><Merch3Alert /></div>
  
	<div class="grid-3col">
		<div class="container">
      <auro-header level="2" display="400">Side nav</auro-header>
    </div>
		<div class="container"><auro-header level="2" display="400">Main - 3 column layout</auro-header><Merch3Alert /></div>
		<div class="container"><auro-header level="2" display="400">Anchor nav</auro-header></div>
	</div>
	<div class="grid-2colSideNav">
		<div class="container"><auro-header level="2" display="400">Side nav</auro-header></div>
		<div class="container"><auro-header level="2" display="400">Main - 2 column layout</auro-header><Merch3Alert /></div>
	</div>
	<div class="grid-2colAnchorNav">
		<div class="container"><auro-header level="2" display="400">Main - 2 column layout</auro-header><Merch3Alert /></div>
		<div class="container"><auro-header level="2" display="400">Anchor nav</auro-header></div>
	</div>
	<div class="grid-2col5050">
		<div class="container"><auro-header level="2" display="400">50/50</auro-header><Merch3Alert /></div>
		<div class="container"><auro-header level="2" display="400">50/50</auro-header><Merch3Alert /></div>
	</div>
	<div class="grid-phones">
		<div class="container"><auro-header level="2" display="400">iPhone Mini</auro-header><Merch3Alert /></div>
		<div class="container"><auro-header level="2" display="400">Galaxy </auro-header><Merch3Alert /></div>
		<div class="container"><auro-header level="2" display="400">iPhone XR</auro-header><p><Merch3Alert /></p></div>
	</div>

	<hr>
	<auro-header level="2" display="800">Deal - Alert</auro-header>
  <auro-header level="2" display="400">Full width</auro-header>
	<div class="container"><Merch3AlertDeal /></div>
  
	<div class="grid-3col">
		<div class="container">
			<auro-header level="2" display="400">Side nav</auro-header>
		</div>
		<div class="container"><auro-header level="2" display="400">Main - 3 column layout</auro-header><Merch3AlertDeal /></div>
		<div class="container"><auro-header level="2" display="400">Anchor nav</auro-header></div>
	</div>
	<div class="grid-2colSideNav">
		<div class="container"><auro-header level="2" display="400">Side nav</auro-header></div>
		<div class="container"><auro-header level="2" display="400">Main - 2 column layout</auro-header><Merch3AlertDeal /></div>
	</div>
	<div class="grid-2colAnchorNav">
		<div class="container"><auro-header level="2" display="400">Main - 2 column layout</auro-header><Merch3AlertDeal /></div>
		<div class="container"><auro-header level="2" display="400">Anchor nav</auro-header></div>
	</div>
	<div class="grid-2col5050">
		<div class="container"><auro-header level="2" display="400">50/50</auro-header><Merch3AlertDeal /></div>
		<div class="container"><auro-header level="2" display="400">50/50</auro-header><Merch3AlertDeal /></div>
	</div>
	<div class="grid-phones">
		<div class="container"><auro-header level="2" display="400">iPhone Mini</auro-header><Merch3AlertDeal /></div>
		<div class="container"><auro-header level="2" display="400">Galaxy </auro-header><Merch3AlertDeal /></div>
		<div class="container"><auro-header level="2" display="400">iPhone XR</auro-header><Merch3AlertDeal /></div>
	</div>

	<hr>
	
	<h2>What's next?</h2>
	
	<ul>
		<li>Create and additional 10-15 different layouts or variants</li>
		<li>Use an API driven approach to change the words, images or colors to create an entirely new offer while using the same code.</li>
		<li>UX copywriters can see what the copy will look like on all placements at once.</li>
		<li>Visual designers can choose colors and images and see how they will look on all placements at once.</li>
	</ul>
</div>

<style>
	.grid-phones {
		display: none;
		background-color: var(--ds-color-background-primary-100-default);
	}
	.grid-3col {
		display: grid;
		gap: 1rem;
		margin-top: 4rem;
	}
  @media (min-width: 1024px) {
	.grid-phones {
		display: grid;
		gap: 2rem;
		margin-top: 4rem;
		grid-template-columns: 320px 360px 375px;
		padding: var(--ds-size-300);
	}
    .grid-3col {
      grid-template-columns: 280px auto 168px;
    }
  }

	.grid-2colSideNav {
		display: grid;
		gap: 1rem;
		margin-top: 4rem;
	}
  @media (min-width: 768px) {
    .grid-2colSideNav {
      grid-template-columns: 280px auto;
    }
  }
	.grid-2colAnchorNav {
		display: grid;
		gap: 1rem;
		margin-top: 4rem;
	}
  @media (min-width: 768px) {
    .grid-2colAnchorNav {
      grid-template-columns: auto 168px;
    }
  }
	.grid-2col5050 {
		display: grid;
		gap: 1rem;
		margin-top: 4rem;
	}
  @media (min-width: 768px) {
    .grid-2col5050 {
      grid-template-columns: 1fr 1fr;
    }
  }
	.mainContent {
		padding: var(--padding);
		display: block;
	}
	.row {
		margin-bottom: 3rem;
	}
	.container {
		container-type: inline-size;
	}
	hr {
		border: .5px dashed #eee;
		margin: 3rem 0;
	}
</style>
