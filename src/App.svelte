<script>
	let isLightTurnOn = true;
	let statusLight = "ON";

	const turn = () => {
		isLightTurnOn = !isLightTurnOn;
		if(isLightTurnOn) {
		statusLight = "ON";
	} else {
		statusLight = "OFF";
	}
	}
</script>

<main>
	<h1>Ter Ok</h1>
	<p>I don't know what is on Ter Nawapol's mind, But are you still OK ?</p>
	<h1>LIGHT: {statusLight}</h1>
	<button on:click={turn}>Ter Nawapol, You should do something.</button>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>