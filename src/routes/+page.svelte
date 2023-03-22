<script>
    const endPlateVideo = '/endPlate.webm';
</script>


<div class="logo">
        <img src="/huppe_logga.png" alt="logo" />
</div>

<div class="container">
    
    <video autoplay loop muted>
        <source src={endPlateVideo} type="video/webm" />
        <track kind="captions">
    </video>
</div>

<style>
    .logo {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        
        
    }
    .logo img{
        position: absolute;
        top: 50%;
        left: 50%;
        max-width: 85%;
        max-height: 85%;
        width: auto;
        height: auto;
        z-index: 100;
        transform: translateX(-50%) translateY(-50%);
    }

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
