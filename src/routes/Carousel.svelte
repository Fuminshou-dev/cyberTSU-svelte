<script>
  import img1 from "$lib/images/1.jpg";
  import img2 from "$lib/images/2.jpg";
  import img3 from "$lib/images/3.jpg";
  import img4 from "$lib/images/4.jpg";
</script>

<div class="carousel hidden md:inline-flex carousel-center h-full flex">
  <div
    id="slide1"
    class="carousel-item flex justify-center align-center relative w-full p-2"
  >
    <img src={img1} alt="team image" class="h-5/6 w-11/12" />
    <div
      class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2"
    >
      <a href="#slide4" class="btn btn-circle">❮</a>
      <a href="#slide2" class="btn btn-circle">❯</a>
    </div>
  </div>
  <div
    id="slide2"
    class="carousel-item flex justify-center align-center relative w-full p-2"
  >
    <img src={img4} alt="team image" class="h-5/6 w-11/12" />
    <div
      class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2"
    >
      <a href="#slide1" class="btn btn-circle">❮</a>
      <a href="#slide3" class="btn btn-circle">❯</a>
    </div>
  </div>
  <div
    id="slide3"
    class="carousel-item flex justify-center align-center relative w-full p-2"
  >
    <img src={img2} alt="team image" class="h-5/6 w-11/12" />
    <div
      class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2"
    >
      <a href="#slide2" class="btn btn-circle">❮</a>
      <a href="#slide4" class="btn btn-circle">❯</a>
    </div>
  </div>
  <div
    id="slide4"
    class="carousel-item flex justify-center align-center relative w-full p-2"
  >
    <img src={img3} alt="team image" class="h-5/6 w-11/12" />
    <div
      class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2"
    >
      <a href="#slide3" class="btn btn-circle">❮</a>
      <a href="#slide1" class="btn btn-circle">❯</a>
    </div>
  </div>
</div>
