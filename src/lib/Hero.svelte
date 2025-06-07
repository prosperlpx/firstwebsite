<script>
  import rocketdab from '../assets/img/rocketdab.png'
</script>

<main>
  <section class="flex flex-col-reverse md:flex-row items-center justify-between my-20 scroll-mt-30 gap-12" id="heros">
    <!-- this is the text area -->
    <div class="max-w-md space-y-4 text-center md:text-left">
      <h1 class="text-5xl sm:text-6xl font-bold">We Boldy Go <span class="text-indigo-300">Where No Rocket</span> Has Gone Before...</h1>
      <p class="text-lg text-slate-300 font-medium">We're building rockets for the next century today. From the moon to Mars, Jupiter and beyond...</p>
      <p class="text-lg text-slate-300 font-medium">Think Acme Rockets.</p>
    </div>

    <!-- this is for the image section -->
     <img src={rocketdab} alt="rocketdab" class="md:max-w-md w-3/4">
  </section>
  <hr class="w-1/2 bg-white mx-auto mt-10">
</main>