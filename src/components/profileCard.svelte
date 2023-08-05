<script>
    import InformationBar from "./informationBar.svelte";
import Tag from "./tag.svelte";

    export let tagList;
    export let communityList;
    export let thumbnailList;
    export let backgroundImageUrl;
    export let bottomBackgroundImageUrl;
    export let portraitImageUrl;
    export let logoIconImageUrl;
</script>

<section class="relative w-[1200px] aspect-[2] bg-[center_center] bg-cover m-auto" 
         style="{backgroundImageUrl ? `background-image: url("${backgroundImageUrl}")` : "background-color: gray"};">
    <header class="box-border w-full h-[14%] bg-[rgba(0,0,0,0.5)] grid grid-cols-[20%_1fr_1fr_2fr] text-[white] border-l-8 border-l-[solid] border-l-[rgb(69,96,229)]">
        <div class="box-border"></div>
        <div class="box-border grid grid-rows-[0.8fr_1fr]">
            <div class="flex items-center w-full italic text-[small] border-b-[rgba(255,255,255,0.7)] border-b border-solid">
                <slot name="title"></slot>
            </div>
            <div class="flex items-center w-full italic text-[x-large] font-[bolder]">
                <slot name="name"></slot>
            </div>
        </div>
        <div class="box-border grid grid-rows-[1fr_1fr] mx-2.5 my-[5px] px-2.5 py-0 border-x-[rgba(255,255,255,0.7)] border-l border-solid border-r">
            <div class="flex items-center w-full">ID:</div>
            <div class="flex items-center w-full text-[x-large] font-[bolder]">
                <slot name="id"></slot>
            </div>
        </div>
        <div class="box-border flex items-end">
            {#each communityList as communityId}
                <img src="images/community_logo/{communityId}.svg" style="width: 50px; filter: invert(100%) sepia(0%) saturate(18%) hue-rotate(319deg) brightness(107%) contrast(104%);" alt={communityId}/>
            {/each}
        </div>
    </header>
    <section class="flex h-[36%] items-center pr-[30px] content-end">
        <img src={logoIconImageUrl} alt="Logo Icon" class="h-[180px] drop-shadow-2xl"/>
    </section>
    <footer class="absolute w-full h-3/6 bg-[center_center] bg-cover bottom-0" 
            style="{bottomBackgroundImageUrl ? `background-image: url("${bottomBackgroundImageUrl}")` : "background-color: gray"};">
        <section class="absolute box-border top-[-15%] w-[82%] h-[15%] flex pb-2.5 left-[18%] items-end">
            {#each tagList as tag}
                <Tag colorHue={tag.colorHue}>
                    <span slot="tagName">{tag.name}</span>
                </Tag>
            {/each}
        </section>
        <div class="box-border w-full h-full bg-[rgba(255,255,255,0.7)] flex items-center">
            <div class="grid items-center gap-[30px] h-4/5 pl-[20%] pr-10" 
                 style="grid-template-columns: repeat({thumbnailList.length}, 1fr);">
            {#each thumbnailList as thumbnailId}
                <img src="images/thumbnails/{thumbnailId}.png" alt={thumbnailId} class="max-w-full"/>
            {/each}
            </div>
        </div>
    </footer>
    <InformationBar 
        portraitImageUrl={portraitImageUrl}>
        <span slot="field1Title">影片數</span>
        <slot name="videoAmount" slot="field1Content" />
        <span slot="field2Title">標誌</span>
        <slot name="logoImage" slot="field2Content" />
        <span slot="field3Title">訂閱數</span>
        <slot name="subscriberAmount" slot="field3Content" />

    </InformationBar>
</section>

<style>
    * {
        font-family: 'Roboto Condensed', 'Noto Sans TC';
        font-weight: 700;
    }
</style>