<script>
  export const prerender = true;
  import "../app.pcss";
  import Footer from "./Footer.svelte";
  import "../app.css";
  import NewNavbar from "./newNavbar.svelte";
</script>

<svelte:head>
  <title>CyberTSU</title>
</svelte:head>

<div class="main flex flex-col h-screen">
  <!-- <Navbar></Navbar> -->
  <NewNavbar />
  <div class="flex-grow mt-20 content-center">
    <slot />
  </div>
  <Footer></Footer>
</div>
