<script>
	import Navbar from "@components/Navbar.svelte";
    import avatar_01 from "$lib/assets/avatar_01.png";
    import avatar_02 from "$lib/assets/avatar_02.png";
    import avatar_03 from "$lib/assets/avatar_03.png";
    import {  } from "$lib/assets/header_bg.avif";
</script>


<header class="p-6">
    <Navbar />
    <section class="grid gap-5 grid-cols-2 mt-5">
        <section class="bg-primary text-black-800 rounded-2xl px-12 py-36 text-center">
            <div>
                <p>Atacama Group</p>
                <h1 class="text-6xl">Saving Nature & Fighting Climate Change Together.</h1>
            </div>
            <div class="mt-8">
                <div class="flex justify-center gap-3">
                    <input class=" bg-white/40 py-4 px-5 block rounded-full" type="email" placeholder="Enter your email">
                    <button class="bg-white py-4 px-5 rounded-full">Subscribe</button>
                </div>
                <div class="mt-5 flex items-center gap-3 justify-center">
                    <div class="flex items-center select-none">
                        <span class="w-8 h-8 rounded-full bg-gray-500 overflow-hidden border-2 border-white"><img src={avatar_01} alt="Avatar 01"></span>
                        <span class="w-8 h-8 -ml-2 rounded-full bg-gray-500  overflow-hidden border-2 border-white"><img src={avatar_02} alt="Avatar 01"></span>
                        <span class="w-8 h-8 -ml-2 rounded-full bg-gray-500  overflow-hidden border-2 border-white"><img src={avatar_03} alt="Avatar 01"></span>
                    </div>
                    <p class="max-w-48 text-left">1.7M+ members of our charity organization</p>
                </div>
            </div>
        </section>
        <section class="bg rounded-2xl">

        </section>
    </section>
</header>

<style>
    .bg {
        background: url("$lib/assets/header_bg.avif");
        background-size: cover;
    }
</style>
