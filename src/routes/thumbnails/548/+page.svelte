<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Code"
    tagList={[data.tagList[1]]}
    backgroundImageUrl="/images/videos/548/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/code_unity_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-c.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground6.png">
    <span slot="subtitle">來實作不同的 Note 功能</span>
    <span slot="title">遊戲 Project RR 製作 <span class="sub-font">#5</span></span>
</VideoThumbnail>