<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Code"
    tagList={[data.tagList[1]]}
    backgroundImageUrl="/images/videos/476/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl=""
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-b.PNG"
    portraitImageUrl="/images/videoThumbnail/headerBackground.png">
    <span slot="subtitle">Lec2a. Higher-order Procedures</span>
    <span slot="title">同步視聽 SICP 公開課 <span class="sub-font">#3</span></span>
</VideoThumbnail>