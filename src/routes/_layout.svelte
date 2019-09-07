<script>
	import Nav from '../components/Nav.svelte';

	export let segment;
</script>

<style>
	main {
		position: relative;
		background-color: #00000022;
		padding: 0.5rem;
		margin: 1rem 3rem;
		box-sizing: border-box;
		min-height: calc(100vh - 7rem);
		display: flex;
	}
	main > section {
		flex: 1;
		background: #ffffff22;
		border-radius: 0.5rem;
		padding: 1rem;
		color: white;
	}
</style>

<Nav {segment}/>

<main>
	<section>
		<slot></slot>
	</section>
</main>