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


  import Button from "./components/Button.svelte";
import Outer from "./components/Outer.svelte";
function handleGreet(event){
	alert(event.detail)
}

</script>

<main>

<Outer on:greet={handleGreet}/>


<Button on:click={()=>alert('clicked')}/>
	<!-- <button on:click={()=>showPopup=true} >Show Popup</button>
	{#if showPopup}
	<Popup on:close={closePopup}/>
	{/if} -->



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