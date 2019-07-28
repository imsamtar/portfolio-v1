<script>
    import Notification from '../components/Notification.svelte';
    let online = true;
    let scrollY = 0;
    let prevScroll = scrollY;
    let showNavbar = true;
    $: showNotification = !online;
    $: showNavbar = scrollY>prevScroll?false:true,prevScroll = scrollY;

</script>

<style>
    nav {
        transition: 1s top;
    }
</style>

<svelte:window bind:online={online} bind:scrollY={scrollY}/>

{#if showNotification}
    <Notification bind:condition={showNotification} color='white' bg='red-500' title='Offline'/>
{/if}

<nav class="bg-black z-10 sticky top-0 h-24" style="top:{showNavbar?'0':'-5.7rem'};">
    <ul class="sm:flex justify-around h-24">
        <li class="flex w-full p-3 sm:p-0"><a class="text-center w-full text-white sm:p-8 font-bold text-lg cursor-pointer hover:bg-white hover:text-black" href="/">Home</a></li>
        <li class="flex w-full p-3 sm:p-0"><a class="text-center w-full text-white sm:p-8 font-bold text-lg cursor-pointer hover:bg-white hover:text-black" href="#projects">Projects</a></li>
        <li class="flex w-full p-3 sm:p-0"><a class="text-center w-full text-white sm:p-8 font-bold text-lg cursor-pointer hover:bg-white hover:text-black" href="#skills">Skills</a></li>
        <li class="flex w-full p-3 sm:p-0"><a class="text-center w-full text-white sm:p-8 font-bold text-lg cursor-pointer hover:bg-white hover:text-black" href="#contact">Contact</a></li>
    </ul>
    <!-- <div class="bg-black text-white">{scrollY} {showNavbar}</div> -->
</nav>
