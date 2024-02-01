<script>
  import Carousel from "./Carousel.svelte";
  import Hero from "./Hero.svelte";
  import img from "$lib/images/be.png";
</script>

<div class="flex place-content-between justify-center items-center m-0">
  <Carousel />
</div>
<h1 class="break-words text-7xl md:hidden pl-5">
  <div class="mockup-phone">
    <div class="camera"></div>
    <div class="display">
      <div class="artboard artboard-demo phone-1">
        <img src={img} alt="CyberTSU logo" />CyberTSU
      </div>
    </div>
  </div>
</h1>
<Hero />
