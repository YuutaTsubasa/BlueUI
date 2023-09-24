<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
  category="Code"
  tagList={[data.tagList[1]]}
  backgroundImageUrl="/images/videos/473/background.png"
  logoUrl="/images/logo.png"
  contentLogoUrl="/images/videos/contentLogos/code_unity_logo.png"
  vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-b.PNG"
  portraitImageUrl="/images/videoThumbnail/headerBackground.png">
  <span slot="subtitle">要來調整攝影機的視角了</span>
  <span slot="title">Unity 開放世界專案 <span class="sub-font">#4</span></span>
</VideoThumbnail>