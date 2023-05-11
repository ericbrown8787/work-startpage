<script>
	import Shortcut from '../lib/shortcut.svelte';
	import { links } from '../lib/config/config.json';
</script>

<svelte:head>
	<title>Home</title>
</svelte:head>
<div class="container">
	<h1>Welcome!</h1>

	<section class="shortcuts">
		<h3>Quick Links</h3>
		<section class="shortcut-links">
			{#each links as link}
				<Shortcut url={link.url} linkLabel={link.label} alt={link.alt} />
			{/each}
		</section>
	</section>
</div>

<style>
	.container {
		padding: 0.5rem;
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	.shortcut-links {
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		gap: 1rem;
	}
</style>
