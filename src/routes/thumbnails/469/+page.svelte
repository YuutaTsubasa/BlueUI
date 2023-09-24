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
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-black.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground.png">
    <span slot="subtitle">順便來試試看一些新玩意</span>
    <span slot="title">初音生日歌回 <span class="sub-font">2023.08.31</span></span>
</VideoThumbnail>