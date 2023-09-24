<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Sing"
    tagList={[data.tagList[2]]}
    backgroundImageUrl="/images/videos/423/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/sing_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-2.0.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground.png"
    volumeNumber=457>
    <span slot="subtitle">來唱唱鋼彈的歌曲吧！</span>
    <span slot="title">GUNDAM 歌回 <span class="sub-font">2023.08.12</span></span>
</VideoThumbnail>