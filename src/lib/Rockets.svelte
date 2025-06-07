<script>
  import rocketlaunch from '../assets/img/rocketlaunch.png';
  import rocketman from '../assets/img/rocketman.png';
  import rocketride from '../assets/img/rocketride.png';
</script>

<main>
  <section id="rockets" class="my-20 scroll-mt-30">
    <h2 class="text-4xl text-center font-bold">Our Rockets</h2>
  <ul class="flex flex-col sm:flex-row items-center justify-between gap-4 sm:gap-8 mt-6">
    <li class="w-1/2 border border-solid border-white p-8 rounded-2xl">
      <img src={rocketlaunch} alt="">
    </li>

    <li class="w-1/2 border border-solid border-white p-8 rounded-2xl">
      <img src={rocketman} alt="">
    </li>

    <li class="w-1/2 border border-solid border-white p-8 rounded-2xl">
      <img src={rocketride} alt="">
    </li>
  </ul>
  </section>
  <hr class="w-1/2 bg-white mx-auto mb-10">
</main>