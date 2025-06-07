<script>
  import Navbar from "./lib/Navbar.svelte";
  import Hero from "./lib/Hero.svelte";
  import Rockets from "./lib/Rockets.svelte";
  import Socials from "./lib/Socials.svelte";
  import Contact from "./lib/Contact.svelte";
  import Footer from "./lib/Footer.svelte";
</script>

<main>
  <Navbar />
  <main class="px-6 max-w-4xl md:mx-auto">
    <Hero />
    <Rockets />
    <Socials />
    <Contact />
  </main>
  <Footer />
</main>