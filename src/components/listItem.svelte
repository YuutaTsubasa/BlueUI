<script>
    import Tag from "./tag.svelte";

    export let item;
    export let coverImageUrl;
    const categoryToColor = {
        "Game": "red",
        "Code": "orange",
        "Sing": "blue",
        "Talk": "green",
        "Null": "null",
    };

    $: categoryColor = categoryToColor[item.category] ?? "gray"

    function formatDate(date) {
        const d = new Date(date);
        let month = '' + (d.getMonth() + 1),
            day = '' + d.getDate(),
            year = d.getFullYear();

        if (month.length < 2) 
            month = '0' + month;
        if (day.length < 2) 
            day = '0' + day;

        return [year, month, day].join('.');
    }
</script>

<section class="grid grid-cols-[3fr_1fr] w-full h-[65px] bg-white">
    <div class="w-full h-full bg-gradient-to-r {`${categoryColor}Gradient`}">
        <div class="h-full flex flex-col items-start justify-center px-5 text-3xl text-white bg-left bg-contain bg-no-repeat pl-8"
             style="background-image: url('/images/schedule/logoIcon.png')">
            <div class="text-lg border-b-2 border-b-white">{formatDate(item.date)} ({new Intl.DateTimeFormat("zh-TW", {weekday: "long"}).format(new Date(item.date)).substring(2)}) {item.time}</div>
            <div>{@html item.name}</div>
        </div>
    </div>
    <div class="relative bg-[rgba(0,0,0,0.3)] h-full flex items-center justify-center z-1">
        <div class="absolute w-full h-full z-2 grayscale bg-cover bg-no-repeat bg-center bg-blend-multiply blur-sm bg-[rgba(0,0,0,0.5)]" style="background-image: url('{coverImageUrl}')"></div>
        <div class="h-full flex items-center justify-center scale-110">
            {#if item.tags.length > 0}
                {#each item.tags as tag}
                    <Tag colorHue={tag.colorHue}><span slot="tagName">{tag.name}</span></Tag>
                {/each}
            {:else}
                <Tag><span slot="tagName">？？</span></Tag>
            {/if}
        </div>
    </div>
</section>

<style>
    .redGradient { @apply from-red-500 to-red-900; }
    .orangeGradient { @apply from-orange-500 to-orange-900; }
    .blueGradient { @apply from-blue-500 to-blue-900; }
    .greenGradient { @apply from-green-500 to-green-900; }
    .grayGradient { @apply from-gray-500 to-gray-900; }
    .nullGradient { @apply from-gray-500 to-gray-900 opacity-50; }


    .redFont { @apply text-red-500; }
    .orangeFont { @apply text-orange-500; }
    .blueFont { @apply text-blue-500; }
    .greenFont { @apply text-green-500; }
    .grayFont { @apply text-gray-500; }

    * {
        font-family: 'Roboto Condensed', 'Noto Sans TC';
        font-weight: 700;
    }
</style>