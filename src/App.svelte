<script>
  //   import ComponentC from "./components/ComponentC.svelte";

  // import Greet from "./components/Greet.svelte";
  // const name="Clark" , heroName="Superman";
  // const obj={
  // 	name:'Barry',
  // 	heroName:'Flash'
  // }

  // import { setContext } from 'svelte'

  // const userName="Pratik";
  // setContext('username-context',userName);

  //   import Popup from "./components/Popup.svelte";
  // 	let showPopup=false;

  // 	function closePopup(event){
  // 		showPopup=false;
  // 		console.log(event.detail)
  // 	}

  //   import Button from "./components/Button.svelte";
  // import Card from "./components/Card.svelte";
  import NameList from "./components/NameList.svelte";
  //   import Outer from "./components/Outer.svelte";
  //   function handleGreet(event) {
  //     alert(event.detail);
  //   }
</script>

<main>


  <NameList>
    <h3 slot="hero" let:firstName let:lastName>{firstName} {lastName}</h3>
  </NameList>
  <NameList>
    <h3 slot="hero" let:firstName let:lastName>{lastName} {firstName}</h3>
  </NameList>
  <NameList>
    <h3 slot="hero" let:firstName let:lastName>{firstName}</h3>
  </NameList>
  <!-- <Outer on:greet={handleGreet} />

  <Button on:click={() => alert("clicked")} /> -->
  <!-- <button on:click={()=>showPopup=true} >Show Popup</button>
	{#if showPopup}
	<Popup on:close={closePopup}/>
	{/if} -->

  <!-- <Card>Card Content</Card>
  <Card>
    <h2>Card Content</h2>
  </Card>
  <Card>
    <img
      src="https://tse1.mm.bing.net/th?id=OIP.DTlxtwyF9mJxHZV-Y1GYVQHaE8&pid=Api&P=0&h=180"
      alt="nature image"
    />
  </Card>
  <Card />


  <Card>
	<div slot="header">
		<h3>Header</h3>
	</div>
	<div slot="content">
		<img
      src="https://tse1.mm.bing.net/th?id=OIP.DTlxtwyF9mJxHZV-Y1GYVQHaE8&pid=Api&P=0&h=180"
      alt="nature image"
    />
	</div>

	<div slot="footer">
		<button>View Details</button>
	</div>
  </Card> -->

  <!-- <h2>App Component UserName - {userName}</h2>
	<ComponentC/> -->

  <!-- <Greet name='Bruce' heroName='batman'/>
	<Greet name={name} heroName={heroName}/>
	<Greet name='Peter Parker'/>
	<Greet {...obj}/> -->
</main>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
