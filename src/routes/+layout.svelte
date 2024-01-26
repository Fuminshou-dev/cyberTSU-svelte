<script>
  import "../app.pcss";
  import Footer from "./Footer.svelte";
  import Navbar from "./Navbar.svelte";
</script>
<svelte:head>
	<title>CyberTSU</title>
</svelte:head>
<Navbar></Navbar>
<slot></slot>
<Footer></Footer>