<script>
	import img1 from "$lib/images/1.jpg"
	import img2 from "$lib/images/2.jpg"
	import img3 from "$lib/images/3.jpg"
	import { Splide, SplideSlide } from '@splidejs/svelte-splide';

import '@splidejs/svelte-splide/css/skyblue';

</script>

<Splide class="splide" options={ { rewind: true, width: 1600 } } aria-label="My Favorite Images">
	<SplideSlide>
	  <img width="1600" src={img1} alt="Image 1"/>
	</SplideSlide>
	<SplideSlide>
	  <img width="1600" src={img2} alt="Image 2"/>
	</SplideSlide>
	<SplideSlide>
		<img width="1600" src={img3} alt="Image 3"/>
	</SplideSlide>
  </Splide>


  <style>
  </style>