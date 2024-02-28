<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Draw"
    tagList={[data.tagList[4]]}
    backgroundImageUrl="/images/videos/537/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/draw_krita_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-c.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground6.png">
    <span slot="subtitle">每月的繪圖練習日到了，照著上次的參考圖繼續畫東西吧！</span>
    <span slot="title">繪圖練習 <span class="sub-font">2024.02.13</span></span>
</VideoThumbnail>