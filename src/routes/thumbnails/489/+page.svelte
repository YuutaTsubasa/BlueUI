<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Game"
    tagList={[data.tagList[0]]}
    backgroundImageUrl="/images/videos/489/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/game_sonic_frontiers_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-fix.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground2.png">
    <span slot="subtitle">Sonic Frontiers (DLC Part)</span>
    <span slot="title">索尼克 未知邊境 <span class="sub-font">#12</span></span>
</VideoThumbnail>