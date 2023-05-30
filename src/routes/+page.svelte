<script>
  import About from "$lib/components/About.svelte";
  import Benefits from "$lib/components/Benefits.svelte";
  import Footer from "$lib/components/Footer.svelte";
  import Header from "$lib/components/Header.svelte";
  import Main from "$lib/components/Main.svelte";
  import Sponsor1 from "../lib/assets/images/sponsor-1.png";
  import Sponsor2 from "../lib/assets/images/sponsor-2.png";
  import Sponsor3 from "../lib/assets/images/sponsor-3.png";
  import Sponsor4 from "../lib/assets/images/sponsor-4.png";
  import Sponsor5 from "../lib/assets/images/sponsor-5.png";
  import event1 from '../lib/assets/images/Rectangle 11.png'
  import event2 from '../lib/assets/images/Rectangle 12.png'
  import event3 from '../lib/assets/images/Rectangle 13.png'
  import event4 from '../lib/assets/images/Rectangle 14.png'
  import event5 from '../lib/assets/images/Rectangle 15.png'
  import event6 from '../lib/assets/images/Rectangle 16.png'
  import Clark from '../lib/assets/images/Clark 1.png'
  import Map from '../lib/assets/images/image 1.png'

  const partner_img_url = [
    '/images/partner_gmv.jpg',
    '/images/partner_RCBC.png',
    '/images/partner_mediacon.jpg',
    '/images/partner_gea.jpg',
    '/images/partner_bw.jpg',
    '/images/partner_attap.jpg',
    '/images/partner_a_planet.png',
  ]

  const events_img_url = [
    '/images/logo_manila.png',
    '/images/logo_north_luzon.png',
    '/images/logo_south_mondanao.png',
    '/images/logo_west_visayas.png',
  ]
</script>
<title>World Travel Expo Philippines - Explore the Best Travel Destinations</title>
<Header />
<Main />
<About />
<Benefits />
<div class="flex flex-col items-center justify-center py-10 px-24">
  <h1 class="text-primary text-4xl mb-2">WORLD TRAVEL EXPO 2023 PARTNERS</h1>
  <div class="flex flex-wrap w-3/4 py-10 gap-6 items-center justify-center">
    {#each partner_img_url as img}
    <img src={img} alt="" class="h-56 w-56 object-scale-down" />
    {/each}
  </div>
  <button
    class="bg-primary text-white font-inika rounded-xl text-2xl px-5 py-1 mt-5"
    >Become a Partner</button
  >
</div>
<div class="flex flex-col py-8 px-24 items-center bg-primary">
  <h1 class="text-white text-4xl mb-10">WORLD TRAVEL EXPO 2023 EVENTS</h1>
  <div class="flex items-center h-36 w-full px-24">
    {#each events_img_url as event_image}

      <img src={event_image} alt="" class="h-full">
    {/each}
  </div>
  <div class="flex h-96 px-24">
    <img src={Clark} alt="" class="w-1/2"/>
    <div class="flex flex-col bg-white p-5">
      <h1 class="text-primary text-3xl mb-1">North Luzon</h1>
      <div class="text-xl">SMX Convention Center Clark Pampanga</div>
      <div class="text-xl my-1">June 16 - 18, 2023</div>
      <p class="text-base text-gray-700 ">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim
        veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
        commodo consequat. Duis aute irure dolor in reprehenderit in voluptate
        velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint
        occaecat cupidatat non proident, sunt in culpa qui officia deserunt
        mollit anim id est laborum.
      </p>
      <button class="bg-primary text-white font-inika w-2/3 mt-auto ml-auto py-2 px-3 rounded-3xl">Join the World Travel Expo 2023</button>
    </div>
  </div>
  <img src={Map} alt="" class="px-24">
</div>
<Footer />
