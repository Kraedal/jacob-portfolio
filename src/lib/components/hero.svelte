<script lang="ts">
  // This script is intentionally left empty for now.
  // You can add any JavaScript functionality here if needed in the future.
  import { fly } from "svelte/transition";
  import { backOut } from "svelte/easing";

  const lines = [
    "Frontend",
    "",
    "Engineer",
    "",
    "+",
    "",
    "UI/UX",
    "",
    "Designer"
  ]
</script>


<section class="mx-auto max-w-7xl sm:px-4 px-8 pt-80 z-40 h-svh " data-hero>
  <div class="grid grid-cols-3 ">
    <div class="grid col-span-2 ">
      <h1 class="text-8xl md:text-9xl font-bold  mb-4 ">JACOB ONG</h1>
      <p class="text-xl md:text-3xl mb-20">Frontend Engineer + UI/UX Designer </p>
      <p class="text-[var(--sage-moss)] underline">Scroll down for more info</p>
    </div>

    <div class="hidden sm:block ">
      <img src="/logo.png" alt="logo" class="rotate-180 hover:rotate-0 transition-transform duration-800 ease-in-out">
    </div>
  </div>


</section>