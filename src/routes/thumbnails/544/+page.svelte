<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Game"
    tagList={[data.tagList[0]]}
    backgroundImageUrl="/images/videos/544/background.jpg"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/game_project_ahnos_ark_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-c.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground6.png">
    <span slot="subtitle">先來玩玩看 DEMO 版吧！</span>
    <span slot="title">倒轉方舟</span>
</VideoThumbnail>