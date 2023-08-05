<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
  category="Code"
  tagList={[data.tagList[1]]}
  backgroundImageUrl="/images/videos/425/background.png"
  logoUrl="/images/logo.png"
  contentLogoUrl="/images/videos/contentLogos/code_unity_logo.png"
  vtuberImageUrl="/images/videos/vtubers/vtuber-2.0.png"
  portraitImageUrl="/images/videoThumbnail/headerBackground.png"
  volumeNumber=425>
  <span slot="subtitle">敵方血量條做完了，接下來該做什麼好呢？</span>
  <span slot="title"><span class="sub-font">嘗試用 </span>Unity <span class="sub-font">製作 </span>動作遊戲 <span class="sub-font">#5</span></span>
</VideoThumbnail>