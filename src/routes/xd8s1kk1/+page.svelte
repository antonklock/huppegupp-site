<script lang="ts">
</script>

<div class="container">
	<video controls={true}>
		<source src="huppe23_Clue_02.mp4" type="video/mp4" />
		<track kind="captions" />
	</video>
	<p>3</p>
</div>

<style>
	.container {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		height: 100vh;
		width: 100%;
		margin: 0;
		padding: 0;
	}

	h1 {
		font-size: 5vw;
		font-weight: 900;
		color: #fff;
		text-shadow: 0 0 10px #000;
		font-family: sans-serif;
		color: red;
	}

	p {
		font-size: 2vw;
		font-weight: 900;
		color: #fff;
		text-shadow: 0 0 10px #000;
		font-family: sans-serif;
		color: yellow;
	}

	video {
		width: 50vw;
		height: auto;
		/* object-fit: cover; */
	}
</style>
