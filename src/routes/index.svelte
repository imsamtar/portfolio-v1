<script>
	import { fade } from 'svelte/transition';
	let clicked = false;
</script>

<style>
	:global(body){background: navy;}
	button {
		background: #280469;
		color: white;
		outline: 0;
		border: 0;
		padding: 10px 15px;
		border-radius: 0.4rem;
	}
</style>

<svelte:head>
	<title>My Portfolio</title>
</svelte:head>

{#if clicked}
	<h1 transition:fade={{delay: 500}}>Great success!</h1>
{:else}
	<button transition:fade={{duration: 500}} on:click={() => clicked = !clicked}>Click</button>
{/if}