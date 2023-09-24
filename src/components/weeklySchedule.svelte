<script>
    import { slide } from 'svelte/transition';
    import { quintOut } from 'svelte/easing';
    import { page } from '$app/stores';
    import ListItem from "./listItem.svelte";

    export let weekNumber;
    export let items;
    export let cover;
    $: number = $page.url.pathname.split("/").findLast(value => value != "");
</script>

<section class="w-[var(--width)] h-[var(--height)] aspect-[var(--aspect-ratio)] mx-auto justify-center
                bg-cover bg-center"
         style="--width: 1200px; --aspect-ratio: calc(1920 / 1080); --height: calc(var(--width) / var(--aspect-ratio));
                background-image: url('/images/schedule/background.png')">
    <div class="w-[var(--width)] h-[var(--height)] aspect-[var(--aspect-ratio)] backdrop-brightness-50 backdrop-blur-sm
                grid grid-rows-[1fr_7fr] justify-center">
        <header class="flex gap-5 m-3 justify-between border-b-2 border-b-white w-[calc(0.95_*_var(--width))]">
            <div class="flex gap-5">
                <h1 class="text-white text-8xl items-center">SCHEDULE</h1>
                <h2 class="grid grid-rows-2 items-end mt-5 mb-3">
                    <span class="text-white text-2xl border-b-white border-b-2 flex items-end justify-center">Week {weekNumber ?? number}</span>
                    <span class="text-white text-xl flex items-end">本週行事曆</span>
                </h2>
            </div>
            <div class="h-full flex items-center">
                <img src="/images/logo.png" alt="Logo" class="h-24"/>
            </div>
        </header>
        <section class="h-full grid grid-cols-[2fr_1fr]">
            <section class="h-full flex flex-col px-3 py-2 gap-2 items-start">
                {#each items as item}
                    <ListItem item={item} coverImageUrl={cover.imageUrl}></ListItem>
                {/each}
            </section>
            <section class="bg-gray-700 mt-2 mb-7 mx-2 bg-cover bg-center flex flex-row items-end justify-center"
                     style="background-image: url('{cover.imageUrl}')">
                
                <div class="bg-[rgba(0,0,0,0.5)] w-full h-10 text-white text-xl flex items-center justify-center">封面繪師：{cover.artist}</div>
            </section>
        </section>
    </div>
</section>

<style>
    /* .redGradient { @apply from-red-500 to-red-900; }
    .orangeGradient { @apply from-orange-500 to-orange-900; }
    .blueGradient { @apply from-blue-500 to-blue-900; }
    .greenGradient { @apply from-green-500 to-green-900; }
    .grayGradient { @apply from-gray-500 to-gray-900; }


    .redFont { @apply text-red-500; }
    .orangeFont { @apply text-orange-500; }
    .blueFont { @apply text-blue-500; }
    .greenFont { @apply text-green-500; }
    .grayFont { @apply text-gray-500; } */

    * {
        font-family: 'Roboto Condensed', 'Noto Sans TC';
        font-weight: 700;
    }
</style>