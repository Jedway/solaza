<script>
  import NavLink from './NavLink.svelte';
  let isMenuOpen = false;
</script>

<header class="fixed w-full bg-gray-900/80 backdrop-blur-sm z-50 border-b border-gray-800">
  <nav class="container mx-auto px-4 py-4 flex justify-between items-center">
    <div class="text-2xl font-bold text-blue-400">Solaza</div>
    
    <!-- Mobile menu button -->
    <button 
      class="md:hidden text-gray-300 hover:text-white"
      on:click={() => isMenuOpen = !isMenuOpen}
    >
      <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
        {#if isMenuOpen}
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"/>
        {:else}
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"/>
        {/if}
      </svg>
    </button>

    <!-- Desktop menu -->
    <div class="hidden md:flex gap-8 items-center">
      <NavLink href="#features">Features</NavLink>
      <NavLink href="#how-it-works">How it Works</NavLink>
      <NavLink href="#contact">Contact</NavLink>
      <button class="btn-primary">
        Get Started
      </button>
    </div>
  </nav>

  <!-- Mobile menu -->
  {#if isMenuOpen}
    <div class="md:hidden px-4 py-2 bg-gray-800 border-t border-gray-700">
      <div class="flex flex-col gap-4 py-4">
        <NavLink href="#features">Features</NavLink>
        <NavLink href="#how-it-works">How it Works</NavLink>
        <NavLink href="#contact">Contact</NavLink>
        <button class="btn-primary w-full">
          Get Started
        </button>
      </div>
    </div>
  {/if}
</header>