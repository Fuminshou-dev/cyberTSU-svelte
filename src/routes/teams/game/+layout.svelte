<script>
  const players = [1, 2, 3, 4, 5];
</script>

<div class="flex flex-col justify-center items-center">
  <slot />
</div>
<div
  class="lg:gap-20 gap-5 grid lg:flex content-center justify-center items-center m-5"
>
  {#each players as player}
    <div
      class="flex flex-col gap-4 h-100 w-60 border border-dashed border-gray-500 p-3 rounded-lg"
    >
      <div class="flex gap-4 items-center">
        <div class="skeleton w-16 h-16 rounded-full shrink-0"></div>
        <div class="flex flex-col gap-4">
          <div class="skeleton h-4 w-20"></div>
          <div class="skeleton h-4 w-28"></div>
        </div>
      </div>
      <div class="skeleton h-32 w-full"></div>
      <button class="btn btn-primary">Подробнее</button>
    </div>
  {/each}
</div>
