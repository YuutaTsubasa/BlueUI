<script>
    export let portraitImageUrl;
</script>


<div class="absolute w-[13%] h-[95%] bg-[center_center] bg-cover shadow-[0px_0px_10px_5px_rgba(0,0,0,0.75)] grid grid-rows-[1fr_50px_200px] left-[3%] inset-y-[2.5%] z-50" 
    style="{portraitImageUrl ? `background-image: url("${portraitImageUrl}")` : "background-color: white"};">
    <div></div>
    <div class="flex items-center justify-between bg-[rgba(255,255,255,0.7)] px-2.5 py-0">
        <div><slot name="field1Title" /></div>
        <div class="text-[x-large] font-[bolder]">
            <slot name="field1Content" />
        </div>
    </div>
    <div class="flex flex-col justify-between bg-[rgb(42,42,42)] text-[rgba(180,180,180,1)] p-2.5">
        <div><slot name="field2Title" /></div>
        <div class="text-center border-b-[rgba(255,255,255,0.7)] border-b border-solid">
            <slot name="field2Content"></slot>
        </div>
        <div><slot name="field3Title" /></div>
        <div class="text-right text-[2em] font-[bolder]">
            <slot name="field3Content"></slot>
        </div>

    </div>
</div>