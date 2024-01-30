<script>
  const players = [1, 2, 3, 4, 5];
</script>

<div class="flex flex-col justify-center items-center">
  <slot />
</div>
<div
  class="gap-10 grid grid-cols-5 content-center justify-center items-center m-10 mt-20"
>
  {#each players as player}
    <div class="flex flex-col gap-4 h-100 w-60 w-52 shadow-xl">
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
