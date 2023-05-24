<script>
    import WteImage from '../assets/images/wte.png'
    import Hero from '../assets/images/hero.png'
</script>
<main class="bg-main flex items-end">
    <div class="pb-20 flex flex-col items-center">
        <img src={WteImage} alt="World Travel Expo" class=" w-2/3">
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
        background-image: url('../assets/images/1.png');
        background-size: cover;
        width: 100%;
        height: 100vh;
    }
</style>