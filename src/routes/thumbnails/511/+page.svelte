<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Game"
    tagList={[data.tagList[0]]}
    backgroundImageUrl="/images/videos/511/background.webp"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/game_exit_8_logo.jpeg"
    vtuberImageUrl="/images/videos/vtubers/vtuber-4.0p.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground3.png">
    <span slot="subtitle">看似恐怖遊戲，實則大家來找碴</span>
    <span slot="title">８番出口 <span class="sub-font">８號出口</span></span>
</VideoThumbnail>