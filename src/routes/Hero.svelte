<script>
    import cyberLogo from '$lib/images/be.png'
</script>


<div class="hero">
        <img src={cyberLogo} alt="">
        <div class="heroText">
            <h1>CyberTSU FTW</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Atque, possimus!</p>
    </div>
</div>


<style>

    .hero {
        background-color: gray;
        display: flex;
        justify-content: center;
        height: 180px;
    }
    .hero * {
        color: black;
        padding: 20px;

    }
    .heroText {
        padding-left: 80px;
        width:400px;
        overflow:hidden;
        height: 150px;
    }
    .hero img {
        width: 150px;
        height: 150px;
    }
</style>