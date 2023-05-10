<script>
	export let url = 'https://www.google.com/';
	export let linkLabel = 'Google';
	import img from './img/alien-icon.svg';
	export let alt = 'An icon';
</script>

<a href={url}>
	<img src={img} {alt} />
	<p>{linkLabel}</p>
</a>

<style>
	img {
		max-width: 50px;
	}
</style>
