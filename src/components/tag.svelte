<script>
    export let colorHue;

    const arrowDistance = "13px"
    const colorSature = "45%";
    $: backgroundColor = `hsl(${colorHue}, ${colorSature}, 50%)`;
</script>

<div class="relative box-border flex items-center z-[2] text-[white] py-0"
     style="height: calc(2 * {arrowDistance}); 
            padding-left: {arrowDistance}; 
            padding-right: calc(1.5 * {arrowDistance});
            background-color: {backgroundColor};">
    <div class="absolute inline-block z-[1] -rotate-45"
         style="padding: calc(0.7 * {arrowDistance});
                left: calc(-0.7 * {arrowDistance}); 
                background-color: {backgroundColor}"></div>
    <slot name="tagName"></slot>
</div>