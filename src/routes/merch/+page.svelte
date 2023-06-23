<script context="module">
	export const prerender = true;
</script>

<script>
	import Merch from '$lib/content/Merch/Merch.svelte';
	import Merch2 from '$lib/content/Merch2/Merch2.svelte';
</script>

<svelte:head>
	<title>Merch: Demo of some of the ways to layout merchandising</title>
</svelte:head>

<div class="mainContent">
	<auro-header>Auro merchandising</auro-header>
	<p>Using container queries so one component can reshape itself into any size needed.</p>
	<auro-header level="2" display="800">Variant 1</auro-header>
  <auro-header level="2" display="400">Full width</auro-header>
	<div class="container"><Merch /></div>
  
	<div class="grid-3col">
		<div class="container">
      <auro-header level="2" display="400">Side nav</auro-header>
      <Merch />
    </div>
		<div class="container"><auro-header level="2" display="400">Main - 3 column layout</auro-header><Merch /></div>
		<div class="container"><auro-header level="2" display="400">Anchor nav</auro-header><Merch /></div>
	</div>
	<div class="grid-2colSideNav">
		<div class="container"><auro-header level="2" display="400">Side nav</auro-header><Merch /></div>
		<div class="container"><auro-header level="2" display="400">Main - 2 column layout</auro-header><Merch /></div>
	</div>
	<div class="grid-2colAnchorNav">
		<div class="container"><auro-header level="2" display="400">Main - 2 column layout</auro-header><Merch /></div>
		<div class="container"><auro-header level="2" display="400">Anchor nav</auro-header><Merch /></div>
	</div>
	<div class="grid-2col5050">
		<div class="container"><auro-header level="2" display="400">50/50</auro-header><Merch /></div>
		<div class="container"><auro-header level="2" display="400">50/50</auro-header><Merch /></div>
	</div>

	<hr>
	<auro-header level="2" display="800">Variant 2</auro-header>
	<p>This variant features a background color and an image overlaying it.  We can add the color to our data file so it can be customized.</p>
	<div class="container"><Merch2 /></div>
	<div class="grid-3col">
		<div class="container"><Merch2 /></div>
		<div class="container"><Merch2 /></div>
		<div class="container"><Merch2 /></div>
	</div>
	<div class="grid-2colSideNav">
		<div class="container"><Merch2 /></div>
		<div class="container"><Merch2 /></div>
	</div>
	<div class="grid-2colAnchorNav">
		<div class="container"><Merch2 /></div>
		<div class="container"><Merch2 /></div>
	</div>
	<div class="grid-2col5050">
		<div class="container"><Merch2 /></div>
		<div class="container"><Merch2 /></div>
	</div>
</div>

<style>
	.grid-3col {
		display: grid;
		gap: 1rem;
		margin-top: 4rem;
	}
  @media (min-width: 1024px) {
    .grid-3col {
      grid-template-columns: 300px auto 200px;
    }
  }

	.grid-2colSideNav {
		display: grid;
		gap: 1rem;
		margin-top: 4rem;
	}
  @media (min-width: 768px) {
    .grid-2colSideNav {
      grid-template-columns: 300px auto;
    }
  }
	.grid-2colAnchorNav {
		display: grid;
		gap: 1rem;
		margin-top: 4rem;
	}
  @media (min-width: 768px) {
    .grid-2colAnchorNav {
      grid-template-columns: auto 200px;
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
	.container-xxs {
		max-width: 140px;
	}

	.container-xs {
		max-width: 200px;
	}

	.container-sm {
		max-width: 360px;
	}

	.container-md {
		max-width: 500px;
	}

	.container-lg {
		max-width: 700px;
	}

	.container-xl {
		max-width: 900px;
	}

	.container-xxl {
		max-width: 1000px;
	}

	.container-xxxl {
		max-width: 1232px;
	}
	hr {
		border: .5px dashed #eee;
		margin: 3rem 0;
	}
</style>
