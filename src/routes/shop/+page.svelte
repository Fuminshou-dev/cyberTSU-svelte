<script>
  let shopItems = [
    {
      title: "Hoodie",
      text: "Cute hoodie",
      img: "IMGURL",
    },
    {
      title: "Shirt",
      text: "Cute shirt",
      img: "IMGURL",
    },
    {
      title: "Pants",
      text: "Cute pants",
      img: "IMGURL",
    },
    {
      title: "Sneakers",
      text: "Cute sneakers",
      img: "IMGURL",
    },
  ];
</script>

<div class="w-full m-0 p-0">
  <div class="flex justify-center items-center self-center md:pl-0">
    <h1 class="font-bold text-3xl">
      Мерч? Можно заказать, чтобы поддержать нашу команду!
    </h1>
  </div>
  <div
    class="gap-10 grid lg:grid-cols-5 content-center justify-center items-center m-10 mt-20"
  >
    {#each shopItems as item}
      <div class="flex flex-col gap-4 w-52">
        <div class="flex justify-center items-center skeleton h-32 w-full">
          {item.img}
        </div>
        <div class="skeleton h-4 w-28">{item.title}</div>
        <div class="skeleton h-4 w-full">{item.text}</div>
        <div class="skeleton h-4 w-full"></div>
        <button class="btn btn-error">Купить</button>
      </div>
    {/each}
  </div>
</div>
