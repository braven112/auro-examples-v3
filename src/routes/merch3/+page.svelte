<script context="module">
	export const prerender = true;
</script>

<script>
	import Merch from '$lib/content/Merch/Merch.svelte';
	import Merch2 from '$lib/content/Merch2/Merch2.svelte';
</script>

<svelte:head>
	<title>Merch: Demo of some of the ways to layout merchandising</title>
	<link rel="stylesheet"
          href="https://fonts.googleapis.com/css?family=Bebas%20Neue">
</svelte:head>

<div class="mainContent">
    <auro-header>Auro merchandising</auro-header>
    <p>Using container queries, one component can reshape itself into any size needed.</p>
    <h2>The problem</h2>
    <p>Currently, we design each merchandising placement independently. This is done because each page is designed independently, and merchandising is often an afterthought. As a result, we find some white space on the page and try to squeeze a merchandising placement there. The result is that each creative is a slightly different size and is only intended to work on the single page it was designed for.</p>
    <h2>Solution</h2>
	
	<ol>
		<li>Standardize our page layouts so we have consistent size columns across the website.</li>
		<li>Then use the new CSS "container" queries to make slight adjustment to each potential placement so that it can reshape itself based on the space available in its given page layout.</li>
	</ol>
    
    <h4>Here are a few highlights worth pointing out...</h4>
    
	<ul>
		<li>Merchandising offers work <u>with</u> our new page layouts</li>
        <li>Easily scale campaigns so that we can offer 100's of personalized offers throughout the site without designing each placement individual</li>
		<li>Design once, use anywhere</li>
		<li>A marketer can decide to place an ad anywhere on our site and it will just work</li>
		<li>Gives the power back to our digital marketers</li>  
    </ul>

	<h2>What am I seeing here?</h2>
	<p>Below you will examples where one merchandising placement (and the exact same code) reshapes itself to fit in any container.</p>
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
