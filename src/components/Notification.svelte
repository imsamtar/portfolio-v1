<script>
    import {onMount} from 'svelte';
    import {fly} from 'svelte/transition';
    export let bg = 'green-500';
    export let color = 'gray-100';
    export let title;
    export let msg;
    export let condition = true;
    onMount(() => {
        setTimeout(() => {
            condition = false;
        },5000);
    })
</script>

<style>
.noti {
    top: 7rem;
    right: 0.5rem;
    min-width: 200px;
}
</style>

<div transition:fly="{{ x: 200, duration: 1000 }}" class="noti inline-block absolute z-40 bg-{bg} text-{color} px-4 py-2 rounded-lg">
{#if title}
    <h3 class="font-bold">{title}</h3>
{/if}
{#if msg}
    <p>{msg}</p>
{/if}
</div>