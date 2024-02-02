<script>
  import Carousel from "./Carousel.svelte";
  import Hero from "./Hero.svelte";
  import img from "$lib/images/be.png";
  import NewCarousel from "./newCarousel.svelte";
</script>

<div
  class="hidden md:flex place-content-between justify-center items-center m-0"
>
  <Carousel />
</div>
<div class="md:hidden"><NewCarousel /></div>
<Hero />
