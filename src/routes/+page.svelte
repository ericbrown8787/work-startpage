<script>
	import Shortcut from '../lib/shortcut.svelte';
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<section class="shortcuts">
	<Shortcut url="https://mail.google.com/" linkLabel="Gmail" alt="Gmail Icon" />
	<Shortcut url="https://www.github.com/" linkLabel="Github" alt="Github Icon" />
</section>

<style>
	.links {
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
	}
</style>
