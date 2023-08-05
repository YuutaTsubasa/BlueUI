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
    vtuberImageUrl="/images/videos/vtubers/vtuber-1.0.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground.png"
    volumeNumber=423>
    <span slot="subtitle">來複習一些以前唱過的 V 家歌曲吧！</span>
    <span slot="title">VOCALOID 歌回 <span class="sub-font">2023.06.18</span></span>
</VideoThumbnail>