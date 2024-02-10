<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Game"
    tagList={[data.tagList[0]]}
    backgroundImageUrl="/images/videos/512/background.jpeg"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/game_sonic_dream_team_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-4.0p2.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground4.png">
    <span slot="subtitle">索尼克新的 Apple Arcade 獨佔遊戲，來玩玩吧</span>
    <span slot="title">Sonic Dream Team <span class="sub-font">#1</span></span>
</VideoThumbnail>