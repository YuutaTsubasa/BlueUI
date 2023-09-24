<script>
  import VideoThumbnail from '../../../components/videoThumbnail.svelte';
  import {data} from '../data';
</script>

<VideoThumbnail 
category="Game"
tagList={[data.tagList[0]]}
backgroundImageUrl="/images/videos/453/background.jpeg"
logoUrl="/images/logo.png"
contentLogoUrl="/images/videos/contentLogos/game_rhythm_sprout_logo.webp"
vtuberImageUrl="/images/videos/vtubers/vtuber-2.0.png"
portraitImageUrl="/images/videoThumbnail/headerBackground.png"
volumeNumber=453>
<span slot="subtitle">來玩玩不一樣的節奏遊戲！</span>
<span slot="title">Rhythm Sprout <span class="sub-font">#1</span></span>
</VideoThumbnail>