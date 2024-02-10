<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Game"
    tagList={[data.tagList[0]]}
    backgroundImageUrl="/images/videos/516/background.jpeg"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/game_melatonin_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-4.0py.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground5.png">
    <span slot="subtitle">一直很想玩的節奏遊戲，今天突發來玩吧！</span>
    <span slot="title">Melatonin</span>
</VideoThumbnail>