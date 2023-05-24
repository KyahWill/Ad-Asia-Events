<script>
  import Footer from "$lib/components/Footer.svelte";
  import Header from "$lib/components/Header.svelte";
  import Main from "$lib/components/Main.svelte";
  import Rectangle from "../../lib/assets/images/Rectangle.png";
  import Skeleton from "../../lib/assets/images/Skeleton.png";
  import Plane from "../../lib/assets/images/Plane.png";
  import Ranking from "../../lib/assets/images/Ranking.png";
  import Hand from "../../lib/assets/images/Hand.png";
  import Horn from "../../lib/assets/images/Horn.png";
  import Group from "../../lib/assets/images/Group.png";
  import write from "../../lib/assets/images/write.png";
</script>

<Header />
<Main />

<!-- why partner -->

<div class="flex flex-col items-center justify-center py-7 px-44 gap-8">
  <h1 class="text-primary text-4xl">WHY PARTNER</h1>
  <div class="border-t border-primary w-full flex">
    <div class="flex flex-col w-full h-full">
      <div class="flex items-center h-full">
        <div class="relative">
          <img src={Rectangle} alt="" class="w-28" />
          <img src={Plane} alt="" class="absolute top-4 left-7 w-10" />
        </div>
        <p class="text-xl ml-5">Explore the Country in One Place</p>
      </div>
      <div class="flex items-center h-full">
        <div class="relative">
          <img src={Rectangle} alt="" class="w-28" />
          <img src={Skeleton} alt="" class="absolute top-4 left-7 w-10" />
        </div>
        <p class="text-xl ml-5">Connect with a Nationwide Audience</p>
      </div>
      <div class="flex items-center h-full">
        <div class="relative">
          <img src={Rectangle} alt="" class="w-28" />
          <img src={Ranking} alt="" class="absolute top-4 left-7 w-10" />
        </div>
        <p class="text-xl ml-5">Gain Exposure and Increase Brand Awareness</p>
      </div>
    </div>
    <div class="flex flex-col w-full h-full">
      <div class="flex items-center h-full">
        <div class="relative">
          <img src={Rectangle} alt="" class="w-28" />
          <img src={Hand} alt="" class="absolute top-4 left-7 w-10" />
        </div>
        <p class="text-xl ml-5">Support a Community of Passionate Travelers</p>
      </div>
      <div class="flex items-center h-full">
        <div class="relative">
          <img src={Rectangle} alt="" class="w-28" />
          <img src={Horn} alt="" class="absolute top-4 left-7 w-10" />
        </div>
        <p class="text-xl ml-5">Promote your Products and Services</p>
      </div>
      <div class="flex items-center h-full">
        <div class="relative">
          <img src={Rectangle} alt="" class="w-28" />
          <img src={Group} alt="" class="absolute top-4 left-7 w-10" />
        </div>
        <p class="text-xl ml-5">Be Part of something BIG</p>
      </div>
    </div>
  </div>
</div>

<!-- Become a partner  -->

<div
  class="bg-primary text-white flex flex-col gap-8 py-9 items-center justify-center px-24"
>
  <h1 class="text-4xl">BECOME A PARTNER</h1>
  <div class="flex w-full gap-5">
    <div class="flex flex-col h-full w-full gap-4">
      <p class="text-sm">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim
        veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
        commodo consequat. Duis aute irure dolor in reprehenderit in voluptate
        velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint
        occaecat cupidatat non proident, sunt in culpa qui officia deserunt
        mollit anim id est laborum. Lorem ipsum dolor sit amet, consectetur
        adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore
        magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
        laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor
        in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
        pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa
        qui officia deserunt mollit anim id est laborum.
      </p>
      <p class="text-sm">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim
        veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
        commodo consequat. Duis aute irure dolor in reprehenderit in voluptate
        velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint
        occaecat cupidatat non proident, sunt in culpa qui officia deserunt
        mollit anim id est laborum. Lorem ipsum dolor sit amet, consectetur
        adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore
        magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
        laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor
        in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
        pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa
        qui officia deserunt mollit anim id est laborum.
      </p>
      <button class="text-primary bg-white px-5 py-1 w-2/6 rounded-2xl">Parnter Inquiry</button>
    </div>
    <div class="w-full">
        <img src={write} alt="" class="" />
    </div>
  </div>
</div>
<Footer />

<style>
</style>
