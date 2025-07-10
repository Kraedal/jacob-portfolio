<script lang="ts">
  import { onMount } from 'svelte';
  
  let isVisible = $state(true);
  
  onMount(() => {
    const handleScroll = () => {
      const heroSection = document.querySelector('section[data-hero]');
      if (heroSection) {
        const heroRect = heroSection.getBoundingClientRect();
        // Hide navigation when hero section is in view
        isVisible = heroRect.top > 0 || heroRect.bottom < window.innerHeight * 0.5;
      }
    };
    
    window.addEventListener('scroll', handleScroll);
    handleScroll(); // Initial check
    
    return () => {
      window.removeEventListener('scroll', handleScroll);
    };
  });
</script>

<section 
  class="sticky top-0 z-50 w-full border-b-2 border-b-white/10 backdrop-blur-md rounded-b-2xl transition-opacity duration-300 ease-in-out"
  class:opacity-0={!isVisible}
  class:opacity-100={isVisible}
>
  <div class="mx-auto max-w-7xl sm:px-2 px-4 py-6">
    <header>
      <div class="flex items-center justify-between">
        <div class="flex items-center">
          <a href="/" class="text-2xl font-bold text-gray-800 ">
            <img src="/image.png" alt="logo" class="h-8 w-16  ">
          </a>
        </div>
        <nav class="flex space-x-4">
          <a href="/home" class=" ">Home</a>
          <a href="/about" class=" ">About</a>
          <a href="/contact" class=" ">Contact</a>
        </nav>
      </div>
    </header>
  </div>
</section>