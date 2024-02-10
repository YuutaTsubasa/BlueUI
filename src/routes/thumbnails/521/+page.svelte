<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Game"
    tagList={[data.tagList[0]]}
    backgroundImageUrl="/images/videos/521/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/game_sonic_dream_team_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-4.0py.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground5.png">
    <span slot="subtitle">今天能完全破關嗎？</span>
    <span slot="title">Sonic Dream Team <span class="sub-font">#4</span></span>
</VideoThumbnail>