<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Code"
    tagList={[data.tagList[1]]}
    backgroundImageUrl="/images/videos/515/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/code_chatgpt_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-4.0py.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground5.png">
    <span slot="subtitle">繼續實作自製的程式語言</span>
    <span slot="title"><span class="sub-font">使用 GPT 輔助</span> 製作程式語言 <span class="sub-font">#4</span></span>
</VideoThumbnail>