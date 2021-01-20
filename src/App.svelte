<script>
	import Main from './Composants/Main.svelte'
	import HowItWorks from './Composants/HowItWorks.svelte'
	import Usage from './Composants/Usage.svelte'

	
</script>

<main>
	<Main />
	<HowItWorks />
	<Usage />
</main>

<style>

@media screen and (max-width: 2200px) {
}

@media screen and (max-width: 800px) {
	main{
           background-color: black;
       }	
}

</style>