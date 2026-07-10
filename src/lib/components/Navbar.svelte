<script lang="ts">
	import { resolve } from '$app/paths';
</script>

<nav>
	<div class="left">
		<a href={resolve('/')} class="link">tagger</a>
		<span class="link">temp</span>
		<span class="link">temp2</span>
	</div>

	<div class="right">
		<span class="link">settings</span>
		<span class="link">user</span>
	</div>
</nav>

<style>
	nav {
		display: flex;
		position: fixed;
		justify-content: space-between;
		z-index: var(--z-navbar);
		top: 0;
		left: 0;
		width: 100%;
		height: var(--navbar-height);
		background-color: var(--color-dark);
	}

	.left {
		display: flex;
		margin-left: 0.5rem;
	}
	.right {
		display: flex;
		margin-right: 0.5rem;
	}

	.link {
		display: flex;
		align-items: center;
		padding: 0.5rem;
		text-decoration: none;
		font-weight: bold;
		color: var(--color-slate);
	}

	.link:hover {
		color: var(--color-cyan);
	}
</style>
