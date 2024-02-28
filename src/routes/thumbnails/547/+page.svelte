<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Sing"
    tagList={[data.tagList[2]]}
    backgroundImageUrl="/images/videos/431/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/sing_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.4-c.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground8.png">
    <span slot="subtitle">嘗試看看唱唱索尼克的歌曲會如何</span>
    <span slot="title">Sonic 索尼克歌回 <span class="sub-font">2024.02.18</span></span>
</VideoThumbnail>