<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
  category="Game"
  tagList={[data.tagList[0]]}
  backgroundImageUrl="/images/videos/430/background.jpeg"
  logoUrl="/images/logo.png"
  contentLogoUrl="/images/videos/contentLogos/game_lost_epic_logo.png"
  vtuberImageUrl="/images/videos/vtubers/vtuber-2.0.png"
  portraitImageUrl="/images/videoThumbnail/headerBackground.png"
  volumeNumber=430>
  <span slot="subtitle">一小時玩遊戲系列復活！</span>
  <span slot="title">失落史詩 LOST EPIC <span class="sub-font">#1</span></span>
</VideoThumbnail>