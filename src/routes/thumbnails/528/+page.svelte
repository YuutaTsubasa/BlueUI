<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Game"
    tagList={[data.tagList[0]]}
    backgroundImageUrl="/images/videos/528/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/game_screamer1_2_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-4.0p3.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground7.png">
    <span slot="subtitle">選舉結束的晚上來玩玩賽車遊戲吧！</span>
    <span slot="title">Screamer 1 & 2</span>
</VideoThumbnail>