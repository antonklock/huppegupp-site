<script>
	const endPlateVideo = '/endPlate_clean.webm';
</script>

<div class="page-content">
	<div class="teams-content">
		<div class="logo">
			<img src="/huppe_logga.png" alt="logo" />
		</div>

		<h1>Teams</h1>

		<div class="teams-container">
			<div class="team-blob" id="flamingo">
				<img src="/flamingo.jpg" alt="flamingo" />
				<h2>Team Flamingo</h2>
				<p class="kapten">Kapten Fabian</p>
				<p>CH</p>
				<p>Ankan</p>
				<p>Hampus</p>
				<p>Albért</p>
			</div>

			<div class="team-blob" id="enhorning">
				<img src="/unicorn.jpg" alt="unicorn" />
				<h2>Team Enhörning</h2>
				<p class="kapten">Kapten Arthur</p>
				<p>Allan</p>
				<p>Emil</p>
				<p>Byström</p>
				<p>Oskar</p>
			</div>
		</div>
	</div>

	<div class="container">
		<video autoplay loop muted playsinline>
			<source src={endPlateVideo} type="video/webm" />
			<track kind="captions" />
		</video>
	</div>

	<footer class="footer">
		<div class="footer-container">
			<h3>The adventure of the year</h3>
			<p>© 2023 Gert Mönsson | Webdesigner | Dreamweaver 2008</p>
		</div>
	</footer>
</div>

<style>
	.page-content {
		display: flex;
		flex-direction: column;
		justify-content: space-between;
		align-items: center;
		height: 100vh;
		width: 100%;
		margin: 0;
		padding: 0;
	}

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
		margin-top: 3rem;
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
		background-color: #0e0e12;
		min-width: 250px;
	}

	.team-blob img {
		height: 8rem;
		width: 8rem;
		border-radius: 10px;
		margin-bottom: 2rem;
		margin-top: 1.5rem;
	}

	.kapten {
		text-decoration: underline;
	}

	.footer {
		display: flex;
		flex-direction: column;
		justify-content: end;
		align-items: center;
		margin-top: 2rem;
		font-family: sans-serif;
		color: red;
	}

	.footer-container {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		height: 100%;
		text-align: center;
	}
	.footer-container h3 {
		margin-bottom: 0;
		text-shadow: 2px 2px 0px #00000077;
	}
	.footer-container p {
		margin-top: 0;
		font-size: small;
		text-shadow: 2px 2px 0px #00000077;
	}
</style>
