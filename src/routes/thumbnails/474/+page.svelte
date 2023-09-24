<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Game"
    tagList={[data.tagList[0]]}
    backgroundImageUrl="/images/videos/474/background.jpeg"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/game_craftopia_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-b.PNG"
    portraitImageUrl="/images/videoThumbnail/headerBackground.png">
    <span slot="subtitle">距上次開的中間有了一次大更新，來玩玩看吧！</span>
    <span slot="title">始世樂土 Craftopia <span class="sub-font">#3</span></span>
</VideoThumbnail>