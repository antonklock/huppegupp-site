<script>
	const endPlateVideo = '/endPlate_clean.webm';
</script>

<div class="logo">
	<img src="/huppe_logga.png" alt="logo" />
</div>

<div class="teams-content">
	<h1>Teams</h1>

	<div class="teams-container">
		<div class="team-blob" id="flamingo">
			<h2>Team Flamingo</h2>
			<p class="kapten">Kapten Fabian</p>
			<p>CH</p>
			<p>Ankan</p>
			<p>Hampus</p>
		</div>

		<div class="team-blob" id="enhorning">
			<h2>Team Enhörning</h2>
			<p class="kapten">Kapten Arthur</p>
			<p>Allan</p>
			<p>Emil</p>
			<p>Byström</p>
		</div>
	</div>
</div>

<div class="container">
	<video autoplay loop muted>
		<source src={endPlateVideo} type="video/webm" />
		<track kind="captions" />
	</video>
</div>

<style>
	.logo {
		display: flex;
		justify-content: center;
		position: sticky;
	}
	.logo img {
		position: relative;
		margin-top: 2rem;
		/* max-width: 55%; */
		max-width: 15em;
		max-height: 85%;
		z-index: 100;
	}

	.container {
		position: fixed;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		overflow: hidden;
		margin: 0;
		padding: 0;
		z-index: -100;
	}

	video {
		position: absolute;
		top: 50%;
		left: 50%;
		min-width: 100%;
		min-height: 100%;
		width: auto;
		height: auto;
		z-index: -100;
		transform: translateX(-50%) translateY(-50%);
		margin: 0;
		padding: 0;
	}

	.teams-content {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}

	.teams-content h1 {
		color: red;
		font-family: sans-serif;
		text-shadow: 2px 2px 0px #000000;
		font-size: 4rem;
		margin-bottom: 1rem;
	}

	.teams-container {
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
		font-family: sans-serif;
		color: red;
		text-shadow: 2px 2px 0px #000000;
	}

	@media only screen and (max-width: 768px) {
		.teams-container {
			flex-direction: column;
		}
	}

	.teams-container h2 {
		color: white;
	}
	.teams-container p {
		text-shadow: none;
		margin-top: 0;
		margin-bottom: 0.5rem;
	}

	.team-blob {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		margin: 1rem;
		padding: 1rem;
		border: 1px solid red;
		border-radius: 0.5rem;
		/* background-color: #131313; */
		/* background-color: white; */

		min-width: 250px;
	}

	#flamingo {
		background-image: url('/flamingo.jpg');
		background-size: cover;
		background-position: center;
		background-repeat: no-repeat;
	}

	#enhorning {
		background-image: url('/unicorn.jpg');
		background-size: cover;
		background-position: center;
		background-repeat: no-repeat;
	}

	.kapten {
		text-decoration: underline;
	}
</style>
