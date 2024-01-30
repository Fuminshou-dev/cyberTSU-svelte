<script>
  const teams = [
    {
      teamTitle: "Dota 2",
      href: "/teams/game/dota2",
      teamText: "Команда по Dota 2",
      img: "https://yt3.googleusercontent.com/ytc/AIf8zZRZZh3EAsdVU9E6Gib_cG59f-1CpwqIUwnaShpeCA=s900-c-k-c0x00ffffff-no-rj",
    },
    {
      teamTitle: "Counter Strike 2",
      href: "/teams/game/cs2",
      teamText: "Команда по CS2",
      img: "https://upload.wikimedia.org/wikipedia/ru/d/db/Counter-strike_2.jpg",
    },
    {
      teamTitle: "Valorant",
      teamText: "Команда по Valorant",
      href: "/teams/game/valorant",
      img: "https://seeklogo.com/images/V/valorant-logo-FAB2CA0E55-seeklogo.com.png",
    },
  ];
</script>

<div class="cards flex m-0 p-0 items-center justify-center gap-20">
  {#each teams as team}
    <div
      class=" outline-dashed outline-slate-500 card w-96 bg-base-50 shadow-2xl"
    >
      <figure class="px-10 pt-10">
        <img src={team.img} alt="Shoes" class="rounded-3xl h-80 w-80" />
      </figure>
      <div class="card-body items-center text-center">
        <h2 class="card-title">{team.teamTitle}</h2>
        <p>{team.teamText}</p>
        <div class="card-actions">
          <a href={team.href}>
            <button class="btn btn-primary">Подробнее</button>
          </a>
        </div>
      </div>
    </div>
  {/each}
</div>
