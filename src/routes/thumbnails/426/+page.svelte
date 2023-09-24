<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
  category="Game"
  tagList={[data.tagList[0]]}
  backgroundImageUrl="/images/videos/426/background.jpeg"
  logoUrl="/images/logo.png"
  contentLogoUrl="/images/videos/contentLogos/game_sonic_origins_plus_logo.png"
  vtuberImageUrl="/images/videos/vtubers/vtuber-2.0.png"
  portraitImageUrl="/images/videoThumbnail/headerBackground.png"
  volumeNumber=426>
  <span slot="subtitle">時隔一年後的加強版，來體驗看看 Game Gear 的遊戲</span>
  <span slot="title">Sonic Origins Plus <span class="sub-font">#1</span></span>
</VideoThumbnail>