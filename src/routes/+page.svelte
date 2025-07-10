
<script lang="ts">
  import NavigationBar from "$lib/components/navigation-bar.svelte";
  import Hero from "$lib/components/hero.svelte";
</script>

<svelte:head>
  <title>Jacob's Portfolio</title>
  <meta name="description" content="Jacob's Portfolio" />
  <link rel="icon" href="/favicon.ico" />
</svelte:head>

<main>
  <NavigationBar />
  <Hero />
  <div class="h-svh"></div>
</main>