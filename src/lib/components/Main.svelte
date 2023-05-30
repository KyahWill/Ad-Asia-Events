<script lang="ts">
    import WteImage from '../assets/images/wte.png'
    import Hero from '../assets/images/hero.png'
    import { onMount } from 'svelte';
    import {slide, fade} from 'svelte/transition'; 
    import {elasticInOut} from 'svelte/easing';

    const bg_urls = [
      '/images/background.jpg',
      '/images/bg_2.jpg'
    ]
    const change_bg = async() =>{
      let counter = 1;
      
      while(true) {

         main.style.backgroundImage = 'url(\''+bg_urls[counter] + '\')'
        await new Promise(r => setTimeout(r, 2000));
         counter = (counter + 1) % bg_urls.length

     } 
    }
    let main: HTMLElement
    onMount(()=> {
     change_bg() 
    })
</script>
<main bind:this={main} class="bg-main flex items-end">
    <div class="pb-20 pt-32 flex flex-col items-center">
        <img src={WteImage} alt="World Travel Expo" class="mt-2 w-2/3">
            <div class="flex gap-5 w-96 items-center justify-center my-7">
                <span class="flex w-5 h-5 bg-white rounded-full cursor-pointer"></span>
                <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span>
                <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span>
                <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span>
                <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span>
                <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span>
                <span class="flex w-5 h-5 bg-gray-200 opacity-60 rounded-full cursor-pointer"></span>
            </div>
            <button class="bg-white text-primary text-2xl px-4 rounded-3xl py-1">
                Join the world Travel Expo 2023
            </button>
    </div>
    <img src={Hero} alt="" class="h-2/3 ml-16">
</main>

<style>
    .bg-main {
        background-image: url('/images/background.jpg');
        background-size: cover;
        width: 100%;
        height: 100vh;
    }
</style>
