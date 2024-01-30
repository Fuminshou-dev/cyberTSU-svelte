<script>
  import { page } from "$app/stores";
  import cyberLogo from "$lib/images/be.png";

  const navs = [
    {
      title: "Главная",
      href: "/",
    },
    {
      title: "Команды",
      href: "/teams",
    },
    {
      title: "О нас",
      href: "/about",
    },
    {
      title: "Контакты",
      href: "/contacts",
    },
    {
      title: "Соц. сети",
      href: "/social",
    },
    {
      title: "Магазин",
      href: "/shop",
    },
    {
      title: "Вакансии",
      href: "/vacancy",
    },
  ];
</script>

<div
  class="navbar overflow-x-auto flex bg-base-100 fixed top-0 z-10 outline outline-slate-500"
>
  <div class="navbar-start">
    <a href="/" class="btn btn-ghost text-xl ml-0">CyberTSU</a>
  </div>
  <div class="navbar-center gap-4">
    {#each navs as { title, href }}
      <a {href} class:active={$page.route.id === href}>{title}</a>
    {/each}
  </div>
  <div class="navbar-end">
    <a href="/">
      <img src={cyberLogo} alt="Cyber tsu logo" class="h-12" />
    </a>
  </div>
</div>

<style>
  .active {
    color: rgba(255, 255, 255, 0.5);
  }
</style>
