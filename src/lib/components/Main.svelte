<script lang="ts">
    import WteImage from '../assets/images/wte.png'
    import Hero from '../assets/images/hero.png'
    import { onMount } from 'svelte';
    import {slide, fade} from 'svelte/transition'; 
    import {elasticInOut} from 'svelte/easing';

    const bg_urls = [
      '/images/background.jpg',
      '/images/bg_2.jpg',
    ]
    const logo_urls = [
      '/images/main_logo.png',
      '/images/main_logo.png'
    ]
    const change_bg = async() =>{
      let counter = 0;
      while(true) {

         main.style.backgroundImage = 'url(\''+bg_urls[counter] + '\')'
        header_logo.src = logo_urls[counter]
        await new Promise(r => setTimeout(r, 3000));
         counter = (counter + 1) % bg_urls.length

     } 
    }
    let main: HTMLElement
    let header_logo: HTMLImageElement
    onMount(()=> {
     change_bg() 
    })
</script>
<main bind:this={main} class="bg-main flex items-center justify-center pt-32">
    <div class="pb-20 flex flex-col items-center">
      <img src="/images/balloon_1.png" alt="baloons" style="position:absolute; top:150px; left:20px;" class="h-20" />
      <img src="/images/balloon_2.png" alt="baloons" style="position:absolute; top:290px; right:30px;" class="h-20" />
      <img src="/images/balloon_3.png" alt="baloons" style="position:absolute; top:500px; left:80px;" class="h-20" />
      <img src="/images/balloon_1.png" alt="baloons" style="position:absolute; top:400px; right:200px;" class="h-28" />
      <img src="/images/balloon_2.png" alt="baloons" style="position:absolute; top:300px; left:200px;" class="h-28" />
      <img bind:this={header_logo} alt="World Travel Expo" class="mt-2 h-96">
            <!-- <div class="flex gap-5 w-96 items-center justify-center my-7"> -->
            <!--     <span class="flex w-5 h-5 bg-white rounded-full cursor-pointer"></span> -->
            <!--     <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span> -->
            <!--     <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span> -->
            <!--     <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span> -->
            <!--     <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span> -->
            <!--     <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span> -->
            <!--     <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span> -->
            <!-- </div> -->
            <button class="bg-white text-primary text-2xl px-4 rounded-3xl py-1">
                Join the World Travel Expo 2023
            </button>
      <img src="/images/city.png" style="position:absolute;bottom:0" />
    </div>
</main>

<style>
    .bg-main {
        background-image: url('/images/background.jpg');
        background-size: cover;
        width: 100%;
        height: 100vh;
    }
</style>
