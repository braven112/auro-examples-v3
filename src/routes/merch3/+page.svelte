<script context="module">
	export const prerender = true;
</script>

<script>
	import Merch1 from '$lib/content/Merch1/Merch1.svelte';
</script>

<svelte:head>
	<title>Merch: Demo of some of the ways to layout merchandising</title>
	<link rel="stylesheet"
          href="https://fonts.googleapis.com/css?family=Bebas%20Neue">
</svelte:head>

<div class="mainContent">
    
	<h2>What am I seeing here?</h2>
	<p>Below you will examples where one merchandising placement (and the exact same code) reshapes itself to fit in any container.</p>
	<auro-header level="2" display="800">Variant 1</auro-header>
  <auro-header level="2" display="400">Full width</auro-header>
	<div class="container"><Merch1 /></div>
  
	<div class="grid-3col">
		<div class="container">
      <auro-header level="2" display="400">Side nav</auro-header>
      <Merch1 />
    </div>
		<div class="container"><auro-header level="2" display="400">Main - 3 column layout</auro-header><Merch1 /></div>
		<div class="container"><auro-header level="2" display="400">Anchor nav</auro-header><Merch1 /></div>
	</div>
	<div class="grid-2colSideNav">
		<div class="container"><auro-header level="2" display="400">Side nav</auro-header><Merch1 /></div>
		<div class="container"><auro-header level="2" display="400">Main - 2 column layout</auro-header><Merch1 /></div>
	</div>
	<div class="grid-2colAnchorNav">
		<div class="container"><auro-header level="2" display="400">Main - 2 column layout</auro-header><Merch1 /></div>
		<div class="container"><auro-header level="2" display="400">Anchor nav</auro-header><Merch1 /></div>
	</div>
	<div class="grid-2col5050">
		<div class="container"><auro-header level="2" display="400">50/50</auro-header><Merch1 /></div>
		<div class="container"><auro-header level="2" display="400">50/50</auro-header><Merch1 /></div>
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
	.grid-3col {
		display: grid;
		gap: 1rem;
		margin-top: 4rem;
	}
  @media (min-width: 1024px) {
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
	.container-xxs {
		max-width: 140px;
	}

	.container-xs {
		max-width: 168px;
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
