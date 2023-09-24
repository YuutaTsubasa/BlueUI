<script>
    import InformationBar from "./informationBar.svelte";
    import Tag from "./tag.svelte";
    import { page } from '$app/stores';

    export let backgroundImageUrl;
    export let logoUrl;
    export let contentLogoUrl;
    export let vtuberImageUrl;
    export let category;
    export let tagList;
    export let volumeNumber;
    export let portraitImageUrl;

    const categoryToColor = {
        "Game": "red",
        "Code": "orange",
        "Sing": "blue",
        "Talk": "green",
        "3D": "cyan",
        "Draw": "pink"
    };

    $: categoryColor = categoryToColor[category] ?? "gray"
    $: number = $page.url.pathname.split("/").findLast(value => value != "");
</script>

<section class="box-border w-[1200px] aspect-[calc(1920_/_1080)] bg-gray-900 mx-auto bg-cover overflow-hidden"
         style="{backgroundImageUrl ? `background-image: url("${backgroundImageUrl}")` : "background-color: rgb(200, 200, 200)"}">
    <section class="box-border w-full h-full grid grid-rows-[28%_1fr] backdrop-brightness-75 backdrop-blur-sm">
        <header class="relative w-full">
            <section class="absolute w-full h-full bg-[position:50%_25%] grayscale z-0" style="background-image: url('/images/videoThumbnail/headerBackground.png')">
            </section>
            <section class="absolute w-full h-full bg-gradient-to-r {categoryColor + "Gradient"} z-10 opacity-75 bg-blend-color-burn">
            </section>
            <!-- <section class="flex items-center w-full h-full">
                <section class="box-border pr-4 py-2 ml-3 bg-gray-200 border-l-[15px] border-l-black z-20">
                    <div class="flex w-max h-full items-center text-black text-3xl pl-2">
                        {`VOL. ${volumeNumber}`}
                    </div>
                </section>
            </section> -->
            <section class="absolute -top-[6px] right-0 w-full h-full flex items-center justify-end">
                <section class="relative box-border pr-4 py-2 ml-3 w-[85%] h-[145px]">
                    <section class="absolute w-full h-full bg-gradient-to-l from-gray-900 opacity-75 z-10">
                    </section>
                    <div class="absolute flex w-full h-full items-center pl-20 gap-5">
                        <div class="w-[15%] h-full flex items-center z-20 ml-10">
                            <img src="/images/logoIcon.png" alt="Logo" class="w-[100%]"/>
                        </div>
                        <div class="grid grid-rows-[1fr_2fr] w-full h-full italic text-left text-white z-20">
                            <div class="thin-font flex items-center border-b-2 border-dashed border-[rgba(255,255,255,0.7)] text-3xl py-2 w-full font-extrabold">
                                <slot name="subtitle"></slot>
                            </div>
                            <div class="thin-font flex items-center text-7xl w-full">
                                <slot name="title"></slot>
                            </div>
                        </div>
                    </div>
                </section>
            </section>
        </header>
        <section class="relative w-full">
            <div class="box-border pl-[250px] grid grid-cols-2 justify-between w-full h-full">
                <div class="flex justify-start items-center pl-20">
                    {#if contentLogoUrl}
                        <img src={contentLogoUrl} alt="Content Logo" class="max-h-[80%] max-w-[80%]"/>
                    {/if}
                </div>
                <div class="flex justify-end items-end">
                    <div class="w-full h-[450px] flex justify-center">
                        {#if vtuberImageUrl}
                            <img src={vtuberImageUrl} alt="Vtuber" class="h-full max-w-none"/>
                        {/if}
                    </div>
                </div>
            </div>
            <footer class="absolute box-border pl-[250px] bottom-0 grid grid-cols-2 items-center justify-between w-full h-[150px]">
                <div class="flex items-end justify-start -mb-10 pl-7 scale-[230%] origin-left">
                    {#each tagList as tag}
                        <Tag colorHue={tag.colorHue}>
                            <span slot="tagName">{tag.name}</span>
                        </Tag>
                    {/each}
                </div>
                <div class="box-border flex justify-end items-center h-full pr-5">
                    <img src={logoUrl} alt="Logo" class="h-[120px]"/>
                </div>
            </footer>
        </section>
        <div class="absolute w-[18%] h-[95%] bg-[center_center] bg-cover shadow-[0px_0px_10px_5px_rgba(0,0,0,0.75)] grid grid-rows-[1fr_200px] left-[3%] inset-y-[2.5%] z-50 bg-white" 
            style="{portraitImageUrl ? `background-image: url("${portraitImageUrl}")` : ""};">
            <div class="overflow-hidden w-full relative">
                <span class="absolute bottom-3 right-[110%] w-max rotate-90 origin-bottom-right text-[60pt] text-right whitespace-nowrap text-[rgba(255,255,255,0.2)] italic">
                    VOL. {volumeNumber ?? number}
                </span>
                <span class="absolute bottom-4 right-[110%] w-max rotate-90 origin-bottom-right text-[60pt] text-right whitespace-nowrap text-[rgba(255,255,255,0.3)] italic">
                    VOL. {volumeNumber ?? number}
                </span>
                <span class="absolute bottom-5 right-[110%] w-max rotate-90 origin-bottom-right text-[60pt] text-right whitespace-nowrap {categoryColor + "Font"} mix-blend-multiply italic">
                    VOL. {volumeNumber ?? number}
                </span>
            </div>
            <!-- <div class="flex items-center justify-between bg-[rgba(255,255,255,0.7)] px-2.5 py-0">
                <div><slot name="field1Title" /></div>
                <div class="text-[x-large] font-[bolder]">
                    <slot name="field1Content" />
                </div>
            </div> -->
            <div class="flex flex-col justify-between bg-[rgb(42,42,42)] text-[rgba(180,180,180,1)] p-2.5">
                <div class="text-center border-b-[rgba(255,255,255,0.7)] border-b border-solid flex items-center justify-center">
                    <img src={logoUrl} alt="Logo" class="h-[100px]"/>
                </div>
                <div class="text-center text-[2.0em] font-[bolder]">
                    VOL. <span class="text-[2em]">{volumeNumber ?? number}</span>
                </div>

            </div>
        </div>
    </section>
</section>

<style>
    .redGradient { @apply from-red-500 to-red-900; }
    .pinkGradient { @apply from-pink-500 to-pink-900; }
    .orangeGradient { @apply from-orange-500 to-orange-900; }
    .cyanGradient { @apply from-cyan-500 to-cyan-900; }
    .blueGradient { @apply from-blue-500 to-blue-900; }
    .greenGradient { @apply from-green-500 to-green-900; }
    .grayGradient { @apply from-gray-500 to-gray-900; }


    .redFont { @apply text-red-500; }
    .pinkFont { @apply text-pink-500; }
    .orangeFont { @apply text-orange-500; }
    .cyanFont { @apply text-cyan-500; }
    .blueFont { @apply text-blue-500; }
    .greenFont { @apply text-green-500; }
    .grayFont { @apply text-gray-500; }

    * {
        font-family: 'Roboto Condensed', 'Noto Sans TC';
        font-weight: 700;
    }

    @font-face {
        font-family: thinFont;
        src: url("/fonts/GlowSansTC-Compressed-Bold.otf");
    }

    :global(.sub-font) {
        /* @apply text-3xl; */
        font-size: 2rem;
        line-height: 2.5rem;
    }

    :global(.two-line-font) {
        @apply text-7xl;
        font-size: 2.75rem;
        line-height: 1;
    }

    :global(.two-line-font .sub-font) {
        font-size: 1.5rem;
        line-height: 0.5rem;
    }

    .thin-font { 
        font-family: 'Roboto Condensed', thinFont;
        --color: black;
        --size: 0.08rem;
        text-shadow: 2px 2px 6px black;
        /* font-weight: lighter !important; */

        /* text-shadow:
            calc(var(--size) * -1) calc(var(--size) * -1) 0 var(--color),
            0        calc(var(--size) * -1) 0 var(--color),
            var(--size) calc(var(--size) * -1) 0 var(--color),
            var(--size)  0        0 var(--color),
            var(--size)  var(--size) 0 var(--color),
            0         var(--size) 0 var(--color),
            calc(var(--size) * -1)  var(--size) 0 var(--color),
            calc(var(--size) * -1)  0        0 var(--color);  */
        /* -webkit-text-stroke: 0.05rem black; */
        
        /* font-family: "twroadfont-1.0";
        font-weight: bolder;
        --color: black;
        --size: 0.06rem;
        text-shadow:
            calc(var(--size) * -1) calc(var(--size) * -1) 0 var(--color),
            0        calc(var(--size) * -1) 0 var(--color),
            var(--size) calc(var(--size) * -1) 0 var(--color),
            var(--size)  0        0 var(--color),
            var(--size)  var(--size) 0 var(--color),
            0         var(--size) 0 var(--color),
            calc(var(--size) * -1)  var(--size) 0 var(--color),
            calc(var(--size) * -1)  0        0 var(--color); */

        /* font-family: "AR FangXinShuH7C80DB5";  */
        /* -webkit-text-stroke: 0.05rem black;  */
        
        /* font-family: "AR SYSongB5HK H32C80";  */
        /* -webkit-text-stroke: 0.05rem black;  */

        /* font-family: "AR UDJingXiHeiE1C80B5HK";  */
        letter-spacing: 0.5pt;
        font-weight: 900;
        /* --color: black;
        --size: 0.08rem;
        text-shadow:
            calc(var(--size) * -1) calc(var(--size) * -1) 0 var(--color),
            0        calc(var(--size) * -1) 0 var(--color),
            var(--size) calc(var(--size) * -1) 0 var(--color),
            var(--size)  0        0 var(--color),
            var(--size)  var(--size) 0 var(--color),
            0         var(--size) 0 var(--color),
            calc(var(--size) * -1)  var(--size) 0 var(--color),
            calc(var(--size) * -1)  0        0 var(--color); */
            
    }
</style>