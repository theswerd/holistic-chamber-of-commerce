<script>
	import Nav from '../components/Nav.svelte';

	export let segment;
</script>

<style>
	main {
		position: relative;
		max-width: 56em;
		background-color: seashell;
		padding: 2em;
		margin: 0 auto;
		box-sizing: border-box;
	}

	:root {
		background-color: darkseagreen;
	}
</style>

<Nav {segment}/>

<main>
	<slot></slot>
</main>