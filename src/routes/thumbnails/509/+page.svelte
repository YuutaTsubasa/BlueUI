<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Code"
    tagList={[data.tagList[1]]}
    backgroundImageUrl="/images/videos/509/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/code_chatgpt_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-fix.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground2.png">
    <span slot="subtitle">精進基本語法 & 嘗試編譯成 JavaScript 的程式碼</span>
    <span slot="title"><span class="sub-font">使用 GPT 輔助</span> 製作程式語言 <span class="sub-font">#3</span></span>
</VideoThumbnail>