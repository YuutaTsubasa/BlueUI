<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
  category="Game"
  tagList={[data.tagList[0]]}
  backgroundImageUrl="/images/videos/437/background.png"
  logoUrl="/images/logo.png"
  contentLogoUrl="/images/videos/contentLogos/game_sonic_origins_plus_logo.png"
  vtuberImageUrl="/images/videos/vtubers/vtuber-2.0.png"
  portraitImageUrl="/images/videoThumbnail/headerBackground.png"
  volumeNumber=437>
  <span slot="subtitle">從【索尼克三重麻煩】繼續體驗 Game Gear 的遊戲</span>
  <span slot="title">Sonic Origins Plus <span class="sub-font">#4</span></span>
</VideoThumbnail>