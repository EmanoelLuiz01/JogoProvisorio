<script>
    import Jogar from './jogar.svelte';
	import Sobre from './sobre.svelte';
	let pagina = "menu";

</script>

<main>
	
</main>

<style>
	.container {
      text-align: center;
    }
</style>

	<div class="container">
	  <button on:click={() => pagina = "jogar"} class="jogar">Jogar</button>
	</div>
	<div>
		<button on:click={() => pagina = "sobre"}>sobre</button>
	</div>
{#if pagina == "jogar"}
	<Jogar />
{:else if pagina == "sobre"}
	<Sobre />		
{/if}


