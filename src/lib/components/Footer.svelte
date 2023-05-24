<script>
        import WteImage from '../assets/images/wte.png'
        import Facebook from '../assets/images/Facebook.png'
        import Twitter from '../assets/images/Twitter.png'
        import Youtube from '../assets/images/Youtube.png'
        import Instagram from '../assets/images/Instagram.png'
</script>
<footer class="bg-secondary flex items-center py-5 px-24 justify-between">
    <div class="flex flex-col items-center">
        <h1 class="text-white font-bold text-">Join our Newsletter</h1>
        <input type="text" placeholder="Name" class="text-center w-60 h-9 rounded-lg my-3 outline-none">
        <input type="text" placeholder="Name" class="text-center w-60 h-9 rounded-lg mb-3 outline-none">
        <button class="font-inika p-1 rounded-3xl bg-primary text-white px-2">Join Now</button>
    </div>
    <img src={WteImage} class="h-48" alt="">
    <ul class="flex flex-col items-start justify-center text-white text-lg">
        <li class="cursor-pointer">Newsroom</li>
        <li class="cursor-pointer">Privacy Policy</li>
        <li class="cursor-pointer">Terms & Conditions</li>
        <li class="font-bold cursor-pointer">Follow us</li>
        <li class="flex w-full gap-3 h-8 my-1">
            <img src={Facebook} alt="" class=" w-9 cursor-pointer">
            <img src={Instagram} alt="" class="w-9 cursor-pointer">
            <img src={Youtube} alt="" class="w-9 cursor-pointer">
            <img src={Twitter} alt="" class="w-9 cursor-pointer">
        </li>
        <li>© All Rights Reserved 2023</li>
    </ul>
</footer>