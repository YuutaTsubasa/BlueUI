<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
  category="Game"
  tagList={[data.tagList[0]]}
  backgroundImageUrl="/images/videos/463/background.png"
  logoUrl="/images/logo.png"
  contentLogoUrl="/images/videos/contentLogos/game_sonic_origins_plus_logo.png"
  vtuberImageUrl="/images/videos/vtubers/vtuber-2.0.png"
  portraitImageUrl="/images/videoThumbnail/headerBackground.png">
  <span slot="subtitle">剩下最後兩款作品了，繼續加油！</span>
  <span slot="title">Sonic Origins Plus <span class="sub-font">#9</span></span>
</VideoThumbnail>