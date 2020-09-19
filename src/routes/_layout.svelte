<script>
	import Nav from '../components/Nav.svelte';

	export let segment;
</script>

<style>
	main {
		position: relative;
		padding: 2em;
		box-sizing: border-box;
		height: 3000px
	}
</style>

<Nav {segment}/>

<main>
	<slot></slot>
</main>