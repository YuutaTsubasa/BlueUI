<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
  category="Game"
  tagList={[data.tagList[0]]}
  backgroundImageUrl="/images/videos/459/background.png"
  logoUrl="/images/logo.png"
  contentLogoUrl="/images/videos/contentLogos/game_sonic_origins_plus_logo.png"
  vtuberImageUrl="/images/videos/vtubers/vtuber-2.0.png"
  portraitImageUrl="/images/videoThumbnail/headerBackground.png"
  volumeNumber=459>
  <span slot="subtitle">來破台【塔爾斯大冒險】了！</span>
  <span slot="title">Sonic Origins Plus <span class="sub-font">#8</span></span>
</VideoThumbnail>