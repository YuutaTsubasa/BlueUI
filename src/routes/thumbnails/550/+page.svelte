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
    <span slot="subtitle">來開歌回囉！</span>
    <span slot="title">2024 年二月底歌回 <span class="sub-font">2024.02.24</span></span>
</VideoThumbnail>