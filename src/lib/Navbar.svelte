<script>
  import {fade} from 'svelte/transition'
  let isMenuOpen = false;
  const toggleMenu = () => {
    isMenuOpen = !isMenuOpen
  }
</script>

  <header class="bg-teal-600 sticky top-0 z-10">
    <section class="max-w-4xl sm:mx-auto sm:py-4 sm:px-6 p-4 flex items-center justify-between" transition:fade>
      <h2 class="text-2xl sm:text-3xl font-bold">
        <a href="#heros">🚀 Acme Rocket</a>
      </h2>
      <!-- this is for the desktop screen -->
       <nav class="hidden sm:inline space-x-6 font-medium text-xl">
        <a href="#rockets" class="hover:opacity-90 active:opacity-70">Rocket</a>
        <a href="#socials" class="hover:opacity-90 active:opacity-70">Socials</a>
        <a href="#contacts" class="hover:opacity-90 active:opacity-70">Contact Us</a>
       </nav>

      {#if !isMenuOpen}
        <button class="sm:hidden text-3xl font-medium cursor-pointer"
          on:click={toggleMenu}
        >
        &#9776;
        </button>
      {:else}
        <button class="sm:hidden text-3xl font-medium cursor-pointer z-20"
          on:click={toggleMenu}
        >
          &times;
        </button>
      {/if}

      {#if isMenuOpen}
        <section class = "absolute sm:hidden  text-5xl font-medium top-0 left-0 bg-black"  transition:fade >
          <button class="flex min-w-screen flex-col items-center min-h-screen right-0 left-0 space-y-16 pt-30" on:click={toggleMenu}>
            <a href="#heros" class=" text-center hover:opacity-90 w-fit">Home</a>
            <a href="#rockets" class=" text-center hover:opacity-90">Our Rockets</a>
            <a href="#socials" class=" text-center hover:opacity-90">Socials</a>
            <a href="#contacts" class=" text-center hover:opacity-90">Contact Us</a>
          </button>
       </section>
      {/if}
    </section>
  </header>
