<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Code"
    tagList={[data.tagList[1]]}
    backgroundImageUrl="/images/videos/519/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/code_unity_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-4.0py.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground5.png">
    <span slot="subtitle">明年希望能有第一個 DEMO 版本的遊戲企劃</span>
    <span slot="title">遊戲 Project RR 製作 <span class="sub-font">#1</span></span>
</VideoThumbnail>