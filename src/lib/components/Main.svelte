<script lang="ts">
    import WteImage from '../assets/images/wte.png'
    import Hero from '../assets/images/hero.png'
    import { onMount } from 'svelte';
    import {slide, fade} from 'svelte/transition'; 
    import {elasticInOut} from 'svelte/easing';
    import { register } from 'swiper/element/bundle';
    // register Swiper custom elements
    const spaceBetween = 10;
    const onProgress = (e) => {
    const [swiper, progress] = e.detail;
      console.log(progress)
    };
    const onSlideChange = (e) => {
      console.log('slide changed')
    }    
    const bg_urls = [
      '/images/background_index.jpg',
      '/images/background_north_luzon.jpg',
      '/images/background_central_visayas.jpg',
      '/images/background_southern_mindanao.jpg',
      '/images/background_western_mindanao.jpg',
      '/images/background_western_visayas.jpg',
      '/images/background_metro_manila.jpg',
    ]
    onMount(()=>{
      register();
    })
    
   </script>
<main class="w-full mt-32">
  <div>
  <swiper-container
    slides-per-view={1}
  space-between={spaceBetween}
  centered-slides={true}
  pagination={{
    hideOnClick: true,
  }}
  navigation={true}
  loop={true}
  speed={500}
  autoplay={{
    delay:3000,
  }}
  on:progress={onProgress}
  on:slidechange={onSlideChange}
  >
    {#each bg_urls as bg_url }
      <swiper-slide>
        <img src={bg_url} alt="location"/>
      </swiper-slide>
    {/each}
  </swiper-container> 
        <button class="absolute bottom-64 right-20 bg-white text-primary mb-16 text-2xl px-4 z-10 rounded-3xl py-1">
          Join the World Travel Expo 2023
        </button>
        <img src="/images/city.png" alt="cities images" style="position:absolute;bottom:180px;right:40px;height:300px; z-index:10;" />
    </div>
  <div class="pb-20 flex flex-col items-center">
    <!-- <div style="position:absolute; top:150px; left:20px;">  -->
    <!--   <img src="/images/balloon_1.png" alt="baloons"  style="position:relative;top:0px;left:0px;" class="baloon h-20" /> -->
    <!-- </div> -->
    <!-- <div style="position:absolute; top:290px; right:30px;" >  -->
    <!--   <img src="/images/balloon_2.png" alt="baloons" style="position:relative;top:0px;left:0px;" class="baloon h-20" /> -->
    <!-- </div> -->
    <!-- <div style="position:absolute; top:500px; left:80px;" >  -->
    <!--   <img src="/images/balloon_3.png" alt="baloons" style="position:relative;top:0px;left:0px;" class="baloon h-20" /> -->
    <!-- </div> -->
    <!-- <div style="position:absolute; top:400px; right:200px;" >  -->
    <!--   <img src="/images/balloon_1.png" alt="baloons" style="position:relative;top:0px;left:0px;" class="baloon h-28" /> -->
    <!-- </div> -->
    <!-- <div style="position:absolute; top:300px; left:200px;" >  -->
    <!--   <img src="/images/balloon_2.png" alt="baloons" style="position:relative;top:0px;left:0px;" class="baloon h-28" /> -->
    <!-- </div> -->
            <!-- <div class="flex gap-5 w-96 items-center justify-center my-7"> -->
            <!--     <span class="flex w-5 h-5 bg-white rounded-full cursor-pointer"></span> -->
            <!--     <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span> -->
            <!--     <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span> -->
            <!--     <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span> -->
            <!--     <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span> -->
            <!--     <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span> -->
            <!--     <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span> -->
            <!-- </div> -->
    </div>
</main>

<style>
    
/* .baloon { */
/*   animation: MoveUpDown 6s linear infinite; */
/* } */

/* @keyframes MoveUpDown { */
/*   0%, 100% { */
/*     top: 0px; */
/*   } */
/*   50% { */
/*     top: 100px; */
/*   } */
/* } */

</style>
