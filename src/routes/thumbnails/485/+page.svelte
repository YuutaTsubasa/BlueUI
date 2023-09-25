<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Game"
    tagList={[data.tagList[0]]}
    backgroundImageUrl="/images/videos/485/background.webp"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/game_horizon_chase_turbo_logo.webp"
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-fix.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground.png">
    <span slot="subtitle">禮拜四說要玩的遊戲，只好今天來開了！</span>
    <span slot="title">Horizon Chase Turbo <span class="sub-font">#1</span></span>
</VideoThumbnail>