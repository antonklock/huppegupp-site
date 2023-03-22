<script>
    const endPlateVideo = '/endPlate.webm';
</script>

<div class="container">
    <video autoplay loop>
        <source src={endPlateVideo} type="video/webm" />
        <track kind="captions">
    </video>

    <div class="content">
        <h1>Page</h1>
        <p>Some content</p>
    </div>
</div>

<style>
    .container {
        position: static;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        overflow: auto;
        margin: 0;
        padding: 0;
    }

    .content {
        color: white;
    }

    video {
        position: relative;
        top: 0%;
        left: 50%;
        min-width: 100%;
        min-height: 100%;
        width: auto;
        height: auto;
        z-index: -100;
        transform: translateX(-50%) translateY(00%);
        margin: 0;
        padding: 0;
    }
</style>
