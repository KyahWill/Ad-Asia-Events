<script lang="ts">
    import WteImage from '../assets/images/wte.png'
    import Hero from '../assets/images/hero.png'
    import { onMount } from 'svelte';
    import {slide, fade} from 'svelte/transition'; 
    import {elasticInOut} from 'svelte/easing';

    const bg_urls = [
      '/images/background_north_luzon.jpg',
      '/images/background_central_visayas.jpg',
      '/images/background_southern_mindanao.jpg',
      '/images/background_western_mindanao.jpg',
      '/images/background_western_visayas.jpg',
      '/images/background_metro_manila.jpg',
    ]

    const change_bg = async() =>{
      let counter = 0;
      while(true) {

         main.style.backgroundImage = 'url(\''+bg_urls[counter] + '\')'
        await new Promise(r => setTimeout(r, 3000));
         counter = (counter + 1) % bg_urls.length

     } 
    }
    let main: HTMLElement
    onMount(()=> {
     change_bg() 
    })
</script>
<main bind:this={main} class="bg-main flex items-end justify-center pt-32">
    <div class="pb-20 flex flex-col items-center">
    <div style="position:absolute; top:150px; left:20px;"> 
      <img src="/images/balloon_1.png" alt="baloons"  style="position:relative;top:0px;left:0px;" class="baloon h-20" />
    </div>
    <div style="position:absolute; top:290px; right:30px;" > 
      <img src="/images/balloon_2.png" alt="baloons" style="position:relative;top:0px;left:0px;" class="baloon h-20" />
    </div>
    <div style="position:absolute; top:500px; left:80px;" > 
      <img src="/images/balloon_3.png" alt="baloons" style="position:relative;top:0px;left:0px;" class="baloon h-20" />
    </div>
    <div style="position:absolute; top:400px; right:200px;" > 
      <img src="/images/balloon_1.png" alt="baloons" style="position:relative;top:0px;left:0px;" class="baloon h-28" />
    </div>
    <div style="position:absolute; top:300px; left:200px;" > 
      <img src="/images/balloon_2.png" alt="baloons" style="position:relative;top:0px;left:0px;" class="baloon h-28" />
    </div>
            <!-- <div class="flex gap-5 w-96 items-center justify-center my-7"> -->
            <!--     <span class="flex w-5 h-5 bg-white rounded-full cursor-pointer"></span> -->
            <!--     <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span> -->
            <!--     <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span> -->
            <!--     <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span> -->
            <!--     <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span> -->
            <!--     <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span> -->
            <!--     <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span> -->
            <!-- </div> -->
            <button class="bg-white text-primary mb-16 text-2xl px-4 rounded-3xl py-1">
                Join the World Travel Expo 2023
            </button>
      <img src="/images/city.png" alt="cities images" style="position:absolute;bottom:0;height:300px" />
    </div>
</main>

<style>
    .bg-main {
        background-image: url('/images/background.jpg');
        background-size: contain;
      background-repeat: no-repeat;
        width: 100%;
        height: 100vh;
    }
.baloon {
  animation: MoveUpDown 6s linear infinite;
}

@keyframes MoveUpDown {
  0%, 100% {
    top: 0px;
  }
  50% {
    top: 100px;
  }
}

</style>
