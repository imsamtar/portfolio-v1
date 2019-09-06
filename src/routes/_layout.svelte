<script>
	import Nav from '../components/Nav.svelte';

	export let segment;
</script>

<style>
	main {
		position: relative;
		max-width: 56em;
		background-color: white;
		padding: 2em;
		margin: 1rem auto;
		box-sizing: border-box;
		min-height: 85vh;
	}
</style>

<Nav {segment}/>

<main>
	<slot></slot>
</main>