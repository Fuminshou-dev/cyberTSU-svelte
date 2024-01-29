<script>
  export const prerender = true;
  import "../app.pcss";
  import Footer from "./Footer.svelte";
  import Navbar from "./Navbar.svelte";
  import "../app.css";
</script>
<svelte:head>
	<title>CyberTSU</title>
</svelte:head>

<div class="main grid grid-rows-[auto_1fr_auto] h-screen">
  <Navbar></Navbar>
  <slot></slot>
  <Footer></Footer>
</div>