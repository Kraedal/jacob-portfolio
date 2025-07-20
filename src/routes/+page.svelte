
<script lang="ts">
  import NavigationBar from "$lib/components/navigation-bar.svelte";
  import Hero from "$lib/components/hero.svelte";
  import About from "$lib/components/about.svelte";
  import Skills from "$lib/components/skills.svelte";
  import Projects from "$lib/components/projects.svelte";
</script>

<svelte:head>
  <title>Jacob Ong — Web Developer & UI/UX Designer</title>
  <meta name="description" content="Hi, I'm Jacob, a web developer who builds modern and aesthetic websites using SvelteKit, TailwindCSS, and more." />
  <meta name="keywords" content="Jacob Ong, web developer, SvelteKit developer, frontend developer, TailwindCSS portfolio, Philippines developer" />
  <meta name="author" content="Jacob Ong" />

  <!-- Open Graph -->
  <meta property="og:title" content="Jacob Ong — Web Developer Portfolio" />
  <meta property="og:description" content="Modern web developer portfolio of Jacob Ong, built with SvelteKit and TailwindCSS." />
  <meta property="og:type" content="website" />
  <meta property="og:url" content="https://jacobong.vercel.app" />
  <meta property="og:image" content="https://jacobong.vercel.app/og-image.png" />

  <!-- Twitter Card -->
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content="Jacob Ong — Web Developer Portfolio" />
  <meta name="twitter:description" content="Modern web developer portfolio of Jacob Ong, built with SvelteKit and TailwindCSS." />
  <meta name="twitter:image" content="https://jacobong.vercel.app/og-image.png" />

  <link rel="icon" href="/favicon.ico" />
  <link rel="canonical" href="https://jacobong.vercel.app/" />
</svelte:head>

<main>
  <NavigationBar />
  <Hero />
  <About />

  <Skills />
  <Projects />
</main>