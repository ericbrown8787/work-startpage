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
		max-height: 100%;
	}
	a {
		display: flex;
		flex-direction: column;
		align-items: center;
		/* justify-content: center; */
		font-size: 1.1rem;
		gap: 5px;
		padding: 15px;
		width: 120px;
		border: 3px solid black;
		border-radius: 10px;
		transition: box-shadow 250ms;
	}

	a p {
		min-width: fit-content;
	}

	a:hover {
		box-shadow: 5px 5px 5px #333;
	}
</style>
