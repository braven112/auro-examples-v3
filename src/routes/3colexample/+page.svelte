<script context="module">
	export const prerender = true;
</script>

<script>
	import Merch3 from '$lib/content/Merch3/Merch3.svelte';
	import Merch3Award from '$lib/content/Merch3/Merch3Award.svelte';
	import Merch3AlertDeal from '$lib/content/Merch3Alert/Merch3AlertDeal.svelte';
</script>

<svelte:head>
	<title>Merch: Demo of some of the ways to layout merchandising</title>
</svelte:head>

<div class="pageLayout-3col">
    <div class="breadcrumbs">
      <auro-nav>
        <auro-breadcrumb href="http://auro.alaskaair.com/components/auro/nav">Home</auro-breadcrumb>
        <auro-breadcrumb href="http://auro.alaskaair.com/components/auro/nav">Level 2</auro-breadcrumb>
        <auro-breadcrumb href="http://auro.alaskaair.com/components/auro/nav">Level 3</auro-breadcrumb>
        <auro-breadcrumb href="http://auro.alaskaair.com/components/auro/nav">Level 4</auro-breadcrumb>
        <auro-breadcrumb>Current</auro-breadcrumb>
      </auro-nav>
    </div>
    <aside class="sidenav">
      <auro-sidenav>
		<span slot="heading">Pet travel policies</span>
		<auro-sidenavitem href="/content/travel-info/pets">Pet travel overview</auro-sidenavitem>
		<auro-sidenavitem href="/content/travel-info/policies/pets-traveling-with-pets/pets-in-cabin">Pets in cabin</auro-sidenavitem>
		<auro-sidenavitem href="/content/travel-info/policies/pets-traveling-with-pets/pets-in-baggage-compartment">Pets in baggage compartment</auro-sidenavitem>
		<auro-sidenavitem href="/content/travel-info/policies/pets-traveling-hawaii">Traveling to Hawaii</auro-sidenavitem>
		<auro-sidenavitem href="/content/travel-info/policies/pets-traveling-international" target="_blank">International travel with pets</auro-sidenavitem>
		<auro-sidenavsection>
		  <span slot="trigger">FAQ</span>
		  <auro-sidenavitem href="/content/travel-info/policies/pets-traveling-with-pets/banfield-qa#safe-to-fly">Is it safe to fly with my pet?</auro-sidenavitem>
		  <auro-sidenavitem href="/content/travel-info/policies/pets-traveling-with-pets/banfield-qa#certain-breeds-prohibited">Why are certain breeds prohibited from flying in the cargo compartment?</auro-sidenavitem>
		  <auro-sidenavitem href="/content/travel-info/policies/pets-traveling-with-pets/banfield-qa#dog-info" target="_blank">Dogs</auro-sidenavitem>
		  <auro-sidenavitem href="/content/travel-info/policies/pets-traveling-with-pets/banfield-qa#cat-info" target="_blank">Cats</auro-sidenavitem>
		</auro-sidenavsection>
	  </auro-sidenav>
	  <Merch3 />
    </aside>
    <main class="main">
      <h1 id="sectionOne">Main Content</h1>
	  <Merch3AlertDeal />
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Consequatur, blanditiis fugiat nisi adipisci totam atque aliquid vero, autem excepturi numquam esse, itaque ab aperiam cum quis! Vel quis excepturi nihil.
      Voluptas exercitationem a provident ducimus temporibus culpa unde cum, cupiditate ab, non autem reprehenderit blanditiis. Eos esse perspiciatis blanditiis nisi suscipit. Quae impedit id tempora ipsa aliquam magni placeat possimus!
      Recusandae sequi, pariatur fugit officia nulla quo veniam nisi adipisci odio consectetur impedit reiciendis beatae culpa labore odit. Aut praesentium dolore qui hic ipsam sint possimus adipisci perferendis quia magnam.
      Doloribus libero minus doloremque commodi, officia incidunt. Consectetur delectus, obcaecati asperiores similique perferendis magni saepe adipisci repellat alias distinctio quam ad dolor nesciunt et voluptatum. Voluptate aspernatur iure exercitationem esse.
      Magni ea tenetur aspernatur eveniet recusandae ratione incidunt a reprehenderit dolor libero vitae, magnam quam, animi accusantium nostrum sit non! Reprehenderit rerum iste quisquam tempore? Dolore praesentium id architecto? Maxime?
      Culpa voluptatibus adipisci inventore obcaecati magnam ullam consequuntur recusandae rem laborum quibusdam, beatae debitis, fugit non dolor ad consectetur iure molestiae illo aspernatur accusamus nulla. Odio autem earum necessitatibus maiores?
      Magni enim et quo repellat adipisci ipsa vero aut exercitationem, suscipit provident quasi officia perferendis possimus perspiciatis nesciunt quae totam ex quam? Adipisci totam corporis asperiores, expedita placeat repellat quis.
      Accusamus, cupiditate pariatur non sit quos minima perspiciatis inventore eveniet expedita obcaecati, harum neque maxime nulla unde. Beatae provident hic perferendis dicta? Ratione doloribus amet, consectetur soluta asperiores reiciendis et?
      Consectetur error esse iusto voluptatem in hic sapiente illo saepe at laborum consequatur sed possimus vitae odit quaerat porro amet, veniam non reiciendis fugit ipsam, eligendi blanditiis! Voluptas, molestiae sed.
      Inventore odit numquam dolorum laborum nulla, id consequuntur suscipit! Expedita alias voluptatum ipsa, cupiditate iusto architecto iure at deserunt corporis? Quod libero ut dolor? Qui sed commodi expedita! Tempora, ad!</p>
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Consequatur, blanditiis fugiat nisi adipisci totam atque aliquid vero, autem excepturi numquam esse, itaque ab aperiam cum quis! Vel quis excepturi nihil.
        Voluptas exercitationem a provident ducimus temporibus culpa unde cum, cupiditate ab, non autem reprehenderit blanditiis. Eos esse perspiciatis blanditiis nisi suscipit. Quae impedit id tempora ipsa aliquam magni placeat possimus!
        Recusandae sequi, pariatur fugit officia nulla quo veniam nisi adipisci odio consectetur impedit reiciendis beatae culpa labore odit. Aut praesentium dolore qui hic ipsam sint possimus adipisci perferendis quia magnam.
        Doloribus libero minus doloremque commodi, officia incidunt. Consectetur delectus, obcaecati asperiores similique perferendis magni saepe adipisci repellat alias distinctio quam ad dolor nesciunt et voluptatum. Voluptate aspernatur iure exercitationem esse.
        Magni ea tenetur aspernatur eveniet recusandae ratione incidunt a reprehenderit dolor libero vitae, magnam quam, animi accusantium nostrum sit non! Reprehenderit rerum iste quisquam tempore? Dolore praesentium id architecto? Maxime?
        Culpa voluptatibus adipisci inventore obcaecati magnam ullam consequuntur recusandae rem laborum quibusdam, beatae debitis, fugit non dolor ad consectetur iure molestiae illo aspernatur accusamus nulla. Odio autem earum necessitatibus maiores?
        Magni enim et quo repellat adipisci ipsa vero aut exercitationem, suscipit provident quasi officia perferendis possimus perspiciatis nesciunt quae totam ex quam? Adipisci totam corporis asperiores, expedita placeat repellat quis.
        Accusamus, cupiditate pariatur non sit quos minima perspiciatis inventore eveniet expedita obcaecati, harum neque maxime nulla unde. Beatae provident hic perferendis dicta? Ratione doloribus amet, consectetur soluta asperiores reiciendis et?
        Consectetur error esse iusto voluptatem in hic sapiente illo saepe at laborum consequatur sed possimus vitae odit quaerat porro amet, veniam non reiciendis fugit ipsam, eligendi blanditiis! Voluptas, molestiae sed.
        Inventore odit numquam dolorum laborum nulla, id consequuntur suscipit! Expedita alias voluptatum ipsa, cupiditate iusto architecto iure at deserunt corporis? Quod libero ut dolor? Qui sed commodi expedita! Tempora, ad!</p>
      <h1 id="sectionTwo">Section Two</h1>
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Consequatur, blanditiis fugiat nisi adipisci totam atque aliquid vero, autem excepturi numquam esse, itaque ab aperiam cum quis! Vel quis excepturi nihil.
        Voluptas exercitationem a provident ducimus temporibus culpa unde cum, cupiditate ab, non autem reprehenderit blanditiis. Eos esse perspiciatis blanditiis nisi suscipit. Quae impedit id tempora ipsa aliquam magni placeat possimus!
        Recusandae sequi, pariatur fugit officia nulla quo veniam nisi adipisci odio consectetur impedit reiciendis beatae culpa labore odit. Aut praesentium dolore qui hic ipsam sint possimus adipisci perferendis quia magnam.
        Doloribus libero minus doloremque commodi, officia incidunt. Consectetur delectus, obcaecati asperiores similique perferendis magni saepe adipisci repellat alias distinctio quam ad dolor nesciunt et voluptatum. Voluptate aspernatur iure exercitationem esse.
        Magni ea tenetur aspernatur eveniet recusandae ratione incidunt a reprehenderit dolor libero vitae, magnam quam, animi accusantium nostrum sit non! Reprehenderit rerum iste quisquam tempore? Dolore praesentium id architecto? Maxime?
        Culpa voluptatibus adipisci inventore obcaecati magnam ullam consequuntur recusandae rem laborum quibusdam, beatae debitis, fugit non dolor ad consectetur iure molestiae illo aspernatur accusamus nulla. Odio autem earum necessitatibus maiores?
        Magni enim et quo repellat adipisci ipsa vero aut exercitationem, suscipit provident quasi officia perferendis possimus perspiciatis nesciunt quae totam ex quam? Adipisci totam corporis asperiores, expedita placeat repellat quis.
        Accusamus, cupiditate pariatur non sit quos minima perspiciatis inventore eveniet expedita obcaecati, harum neque maxime nulla unde. Beatae provident hic perferendis dicta? Ratione doloribus amet, consectetur soluta asperiores reiciendis et?
        Consectetur error esse iusto voluptatem in hic sapiente illo saepe at laborum consequatur sed possimus vitae odit quaerat porro amet, veniam non reiciendis fugit ipsam, eligendi blanditiis! Voluptas, molestiae sed.
        Inventore odit numquam dolorum laborum nulla, id consequuntur suscipit! Expedita alias voluptatum ipsa, cupiditate iusto architecto iure at deserunt corporis? Quod libero ut dolor? Qui sed commodi expedita! Tempora, ad!</p>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Consequatur, blanditiis fugiat nisi adipisci totam atque aliquid vero, autem excepturi numquam esse, itaque ab aperiam cum quis! Vel quis excepturi nihil.
          Voluptas exercitationem a provident ducimus temporibus culpa unde cum, cupiditate ab, non autem reprehenderit blanditiis. Eos esse perspiciatis blanditiis nisi suscipit. Quae impedit id tempora ipsa aliquam magni placeat possimus!
          Recusandae sequi, pariatur fugit officia nulla quo veniam nisi adipisci odio consectetur impedit reiciendis beatae culpa labore odit. Aut praesentium dolore qui hic ipsam sint possimus adipisci perferendis quia magnam.
          Doloribus libero minus doloremque commodi, officia incidunt. Consectetur delectus, obcaecati asperiores similique perferendis magni saepe adipisci repellat alias distinctio quam ad dolor nesciunt et voluptatum. Voluptate aspernatur iure exercitationem esse.
          Magni ea tenetur aspernatur eveniet recusandae ratione incidunt a reprehenderit dolor libero vitae, magnam quam, animi accusantium nostrum sit non! Reprehenderit rerum iste quisquam tempore? Dolore praesentium id architecto? Maxime?
          Culpa voluptatibus adipisci inventore obcaecati magnam ullam consequuntur recusandae rem laborum quibusdam, beatae debitis, fugit non dolor ad consectetur iure molestiae illo aspernatur accusamus nulla. Odio autem earum necessitatibus maiores?
          Magni enim et quo repellat adipisci ipsa vero aut exercitationem, suscipit provident quasi officia perferendis possimus perspiciatis nesciunt quae totam ex quam? Adipisci totam corporis asperiores, expedita placeat repellat quis.
          Accusamus, cupiditate pariatur non sit quos minima perspiciatis inventore eveniet expedita obcaecati, harum neque maxime nulla unde. Beatae provident hic perferendis dicta? Ratione doloribus amet, consectetur soluta asperiores reiciendis et?
          Consectetur error esse iusto voluptatem in hic sapiente illo saepe at laborum consequatur sed possimus vitae odit quaerat porro amet, veniam non reiciendis fugit ipsam, eligendi blanditiis! Voluptas, molestiae sed.
          Inventore odit numquam dolorum laborum nulla, id consequuntur suscipit! Expedita alias voluptatum ipsa, cupiditate iusto architecto iure at deserunt corporis? Quod libero ut dolor? Qui sed commodi expedita! Tempora, ad!</p>
        <h1 id="sectionThree">Section Three</h1>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Consequatur, blanditiis fugiat nisi adipisci totam atque aliquid vero, autem excepturi numquam esse, itaque ab aperiam cum quis! Vel quis excepturi nihil.
          Voluptas exercitationem a provident ducimus temporibus culpa unde cum, cupiditate ab, non autem reprehenderit blanditiis. Eos esse perspiciatis blanditiis nisi suscipit. Quae impedit id tempora ipsa aliquam magni placeat possimus!
          Recusandae sequi, pariatur fugit officia nulla quo veniam nisi adipisci odio consectetur impedit reiciendis beatae culpa labore odit. Aut praesentium dolore qui hic ipsam sint possimus adipisci perferendis quia magnam.
          Doloribus libero minus doloremque commodi, officia incidunt. Consectetur delectus, obcaecati asperiores similique perferendis magni saepe adipisci repellat alias distinctio quam ad dolor nesciunt et voluptatum. Voluptate aspernatur iure exercitationem esse.
          Magni ea tenetur aspernatur eveniet recusandae ratione incidunt a reprehenderit dolor libero vitae, magnam quam, animi accusantium nostrum sit non! Reprehenderit rerum iste quisquam tempore? Dolore praesentium id architecto? Maxime?
          Culpa voluptatibus adipisci inventore obcaecati magnam ullam consequuntur recusandae rem laborum quibusdam, beatae debitis, fugit non dolor ad consectetur iure molestiae illo aspernatur accusamus nulla. Odio autem earum necessitatibus maiores?
          Magni enim et quo repellat adipisci ipsa vero aut exercitationem, suscipit provident quasi officia perferendis possimus perspiciatis nesciunt quae totam ex quam? Adipisci totam corporis asperiores, expedita placeat repellat quis.
          Accusamus, cupiditate pariatur non sit quos minima perspiciatis inventore eveniet expedita obcaecati, harum neque maxime nulla unde. Beatae provident hic perferendis dicta? Ratione doloribus amet, consectetur soluta asperiores reiciendis et?
          Consectetur error esse iusto voluptatem in hic sapiente illo saepe at laborum consequatur sed possimus vitae odit quaerat porro amet, veniam non reiciendis fugit ipsam, eligendi blanditiis! Voluptas, molestiae sed.
          Inventore odit numquam dolorum laborum nulla, id consequuntur suscipit! Expedita alias voluptatum ipsa, cupiditate iusto architecto iure at deserunt corporis? Quod libero ut dolor? Qui sed commodi expedita! Tempora, ad!</p>
          <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Consequatur, blanditiis fugiat nisi adipisci totam atque aliquid vero, autem excepturi numquam esse, itaque ab aperiam cum quis! Vel quis excepturi nihil.
            Voluptas exercitationem a provident ducimus temporibus culpa unde cum, cupiditate ab, non autem reprehenderit blanditiis. Eos esse perspiciatis blanditiis nisi suscipit. Quae impedit id tempora ipsa aliquam magni placeat possimus!
            Recusandae sequi, pariatur fugit officia nulla quo veniam nisi adipisci odio consectetur impedit reiciendis beatae culpa labore odit. Aut praesentium dolore qui hic ipsam sint possimus adipisci perferendis quia magnam.
            Doloribus libero minus doloremque commodi, officia incidunt. Consectetur delectus, obcaecati asperiores similique perferendis magni saepe adipisci repellat alias distinctio quam ad dolor nesciunt et voluptatum. Voluptate aspernatur iure exercitationem esse.
            Magni ea tenetur aspernatur eveniet recusandae ratione incidunt a reprehenderit dolor libero vitae, magnam quam, animi accusantium nostrum sit non! Reprehenderit rerum iste quisquam tempore? Dolore praesentium id architecto? Maxime?
            Culpa voluptatibus adipisci inventore obcaecati magnam ullam consequuntur recusandae rem laborum quibusdam, beatae debitis, fugit non dolor ad consectetur iure molestiae illo aspernatur accusamus nulla. Odio autem earum necessitatibus maiores?
            Magni enim et quo repellat adipisci ipsa vero aut exercitationem, suscipit provident quasi officia perferendis possimus perspiciatis nesciunt quae totam ex quam? Adipisci totam corporis asperiores, expedita placeat repellat quis.
            Accusamus, cupiditate pariatur non sit quos minima perspiciatis inventore eveniet expedita obcaecati, harum neque maxime nulla unde. Beatae provident hic perferendis dicta? Ratione doloribus amet, consectetur soluta asperiores reiciendis et?
            Consectetur error esse iusto voluptatem in hic sapiente illo saepe at laborum consequatur sed possimus vitae odit quaerat porro amet, veniam non reiciendis fugit ipsam, eligendi blanditiis! Voluptas, molestiae sed.
            Inventore odit numquam dolorum laborum nulla, id consequuntur suscipit! Expedita alias voluptatum ipsa, cupiditate iusto architecto iure at deserunt corporis? Quod libero ut dolor? Qui sed commodi expedita! Tempora, ad!</p>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Consequatur, blanditiis fugiat nisi adipisci totam atque aliquid vero, autem excepturi numquam esse, itaque ab aperiam cum quis! Vel quis excepturi nihil.
              Voluptas exercitationem a provident ducimus temporibus culpa unde cum, cupiditate ab, non autem reprehenderit blanditiis. Eos esse perspiciatis blanditiis nisi suscipit. Quae impedit id tempora ipsa aliquam magni placeat possimus!
              Recusandae sequi, pariatur fugit officia nulla quo veniam nisi adipisci odio consectetur impedit reiciendis beatae culpa labore odit. Aut praesentium dolore qui hic ipsam sint possimus adipisci perferendis quia magnam.
              Doloribus libero minus doloremque commodi, officia incidunt. Consectetur delectus, obcaecati asperiores similique perferendis magni saepe adipisci repellat alias distinctio quam ad dolor nesciunt et voluptatum. Voluptate aspernatur iure exercitationem esse.
              Magni ea tenetur aspernatur eveniet recusandae ratione incidunt a reprehenderit dolor libero vitae, magnam quam, animi accusantium nostrum sit non! Reprehenderit rerum iste quisquam tempore? Dolore praesentium id architecto? Maxime?
              Culpa voluptatibus adipisci inventore obcaecati magnam ullam consequuntur recusandae rem laborum quibusdam, beatae debitis, fugit non dolor ad consectetur iure molestiae illo aspernatur accusamus nulla. Odio autem earum necessitatibus maiores?
              Magni enim et quo repellat adipisci ipsa vero aut exercitationem, suscipit provident quasi officia perferendis possimus perspiciatis nesciunt quae totam ex quam? Adipisci totam corporis asperiores, expedita placeat repellat quis.
              Accusamus, cupiditate pariatur non sit quos minima perspiciatis inventore eveniet expedita obcaecati, harum neque maxime nulla unde. Beatae provident hic perferendis dicta? Ratione doloribus amet, consectetur soluta asperiores reiciendis et?
              Consectetur error esse iusto voluptatem in hic sapiente illo saepe at laborum consequatur sed possimus vitae odit quaerat porro amet, veniam non reiciendis fugit ipsam, eligendi blanditiis! Voluptas, molestiae sed.
              Inventore odit numquam dolorum laborum nulla, id consequuntur suscipit! Expedita alias voluptatum ipsa, cupiditate iusto architecto iure at deserunt corporis? Quod libero ut dolor? Qui sed commodi expedita! Tempora, ad!</p>
              <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Consequatur, blanditiis fugiat nisi adipisci totam atque aliquid vero, autem excepturi numquam esse, itaque ab aperiam cum quis! Vel quis excepturi nihil.
                Voluptas exercitationem a provident ducimus temporibus culpa unde cum, cupiditate ab, non autem reprehenderit blanditiis. Eos esse perspiciatis blanditiis nisi suscipit. Quae impedit id tempora ipsa aliquam magni placeat possimus!
                Recusandae sequi, pariatur fugit officia nulla quo veniam nisi adipisci odio consectetur impedit reiciendis beatae culpa labore odit. Aut praesentium dolore qui hic ipsam sint possimus adipisci perferendis quia magnam.
                Doloribus libero minus doloremque commodi, officia incidunt. Consectetur delectus, obcaecati asperiores similique perferendis magni saepe adipisci repellat alias distinctio quam ad dolor nesciunt et voluptatum. Voluptate aspernatur iure exercitationem esse.
                Magni ea tenetur aspernatur eveniet recusandae ratione incidunt a reprehenderit dolor libero vitae, magnam quam, animi accusantium nostrum sit non! Reprehenderit rerum iste quisquam tempore? Dolore praesentium id architecto? Maxime?
                Culpa voluptatibus adipisci inventore obcaecati magnam ullam consequuntur recusandae rem laborum quibusdam, beatae debitis, fugit non dolor ad consectetur iure molestiae illo aspernatur accusamus nulla. Odio autem earum necessitatibus maiores?
                Magni enim et quo repellat adipisci ipsa vero aut exercitationem, suscipit provident quasi officia perferendis possimus perspiciatis nesciunt quae totam ex quam? Adipisci totam corporis asperiores, expedita placeat repellat quis.
                Accusamus, cupiditate pariatur non sit quos minima perspiciatis inventore eveniet expedita obcaecati, harum neque maxime nulla unde. Beatae provident hic perferendis dicta? Ratione doloribus amet, consectetur soluta asperiores reiciendis et?
                Consectetur error esse iusto voluptatem in hic sapiente illo saepe at laborum consequatur sed possimus vitae odit quaerat porro amet, veniam non reiciendis fugit ipsam, eligendi blanditiis! Voluptas, molestiae sed.
                Inventore odit numquam dolorum laborum nulla, id consequuntur suscipit! Expedita alias voluptatum ipsa, cupiditate iusto architecto iure at deserunt corporis? Quod libero ut dolor? Qui sed commodi expedita! Tempora, ad!</p>
          <h1 id="sectionFour">Section Four</h1>
          <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Consequatur, blanditiis fugiat nisi adipisci totam atque aliquid vero, autem excepturi numquam esse, itaque ab aperiam cum quis! Vel quis excepturi nihil.
            Voluptas exercitationem a provident ducimus temporibus culpa unde cum, cupiditate ab, non autem reprehenderit blanditiis. Eos esse perspiciatis blanditiis nisi suscipit. Quae impedit id tempora ipsa aliquam magni placeat possimus!
            Recusandae sequi, pariatur fugit officia nulla quo veniam nisi adipisci odio consectetur impedit reiciendis beatae culpa labore odit. Aut praesentium dolore qui hic ipsam sint possimus adipisci perferendis quia magnam.
            Doloribus libero minus doloremque commodi, officia incidunt. Consectetur delectus, obcaecati asperiores similique perferendis magni saepe adipisci repellat alias distinctio quam ad dolor nesciunt et voluptatum. Voluptate aspernatur iure exercitationem esse.
            Magni ea tenetur aspernatur eveniet recusandae ratione incidunt a reprehenderit dolor libero vitae, magnam quam, animi accusantium nostrum sit non! Reprehenderit rerum iste quisquam tempore? Dolore praesentium id architecto? Maxime?
            Culpa voluptatibus adipisci inventore obcaecati magnam ullam consequuntur recusandae rem laborum quibusdam, beatae debitis, fugit non dolor ad consectetur iure molestiae illo aspernatur accusamus nulla. Odio autem earum necessitatibus maiores?
            Magni enim et quo repellat adipisci ipsa vero aut exercitationem, suscipit provident quasi officia perferendis possimus perspiciatis nesciunt quae totam ex quam? Adipisci totam corporis asperiores, expedita placeat repellat quis.
            Accusamus, cupiditate pariatur non sit quos minima perspiciatis inventore eveniet expedita obcaecati, harum neque maxime nulla unde. Beatae provident hic perferendis dicta? Ratione doloribus amet, consectetur soluta asperiores reiciendis et?
            Consectetur error esse iusto voluptatem in hic sapiente illo saepe at laborum consequatur sed possimus vitae odit quaerat porro amet, veniam non reiciendis fugit ipsam, eligendi blanditiis! Voluptas, molestiae sed.
            Inventore odit numquam dolorum laborum nulla, id consequuntur suscipit! Expedita alias voluptatum ipsa, cupiditate iusto architecto iure at deserunt corporis? Quod libero ut dolor? Qui sed commodi expedita! Tempora, ad!</p>
    </main>
    <aside class="anchornav">
      <auro-nav anchorNavContent=".main">
        <span slot="label">Anchor Navigation</span>
        <span slot="mobileToggleCollapsed">View More</span>
        <span slot="mobileToggleExpanded">View Less</span>
        <auro-anchorlink href="#sectionOne">Section 1</auro-anchorlink>
        <auro-anchorlink href="#sectionTwo">Section 2</auro-anchorlink>
        <auro-anchorlink href="#sectionThree">Section 3</auro-anchorlink>
        <auro-anchorlink href="#sectionFour">Section 4</auro-anchorlink>
      </auro-nav>
	  <Merch3Award />
    </aside>
  </div>

<style>
		  @import "./../../lib/wcss-grid.css";
	hr {
		border: .5px dashed #eee;
		margin: 3rem 0;
	}
</style>
