<script lang="ts">
	import '@fontsource-variable/inter/wght.css';
	import '../app.css';
	import Navbar from '$lib/components/Navbar.svelte';

	let { children } = $props();
</script>

<Navbar />

<main>
	{@render children()}
</main>

<style>
	main {
		padding: var(--navbar-height) 1rem 0;
	}
</style>
