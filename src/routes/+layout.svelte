<script lang="ts">
	import Navbar from '$lib/components/Navbar.svelte';
	import '../app.css';

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
