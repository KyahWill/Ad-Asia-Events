<script>
    import rightArrow from '../assets/images/icon.png'
</script>
<header class="bg-transparent h-20 flex items-center justify-between font-inika absolute  top-0 left-0 w-screen px-24 z-10">
  <h1 class=" text-2xl text-primary">WORLD TRAVEL EXPO</h1>
 <hr class="hr">
  <ul class="flex items-center gap-9 font-normal">
    <a href="/"> <li class="text-white text-2xl cursor-pointer">About</li> </a>
    <a href="/Partners"><li class="text-white text-2xl cursor-pointer">Partners</li> </a>
    <li class="text-white text-2xl flex items-center gap-2 cursor-pointer">Events <img src={rightArrow} alt="arrow" class="w-3"></li>
    <li class="text-white text-2xl cursor-pointer">Contact Us</li>
  </ul>
  <button class="text-primary bg-transparent border-2 border-primary font-inika text-2xl w-32 h-12 rounded-3xl leading-8">Register</button>
</header>

<style>
    .hr {
        position: absolute;
        top: 80px;
        width: 1350px;
        left: 95px;
        height: 2px;
    }
</style>
