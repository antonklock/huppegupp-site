<script>
    const endPlateVideo = '/endPlate.webm';
</script>

<div class="container">
    <video autoplay loop muted>
        <source src={endPlateVideo} type="video/webm" />
        <track kind="captions">
    </video>
</div>

<style>
    .container {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        overflow: hidden;
        margin: 0;
        padding: 0;
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
</style>
