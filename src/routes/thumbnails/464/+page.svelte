<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
  category="Code"
  tagList={[data.tagList[1]]}
  backgroundImageUrl="/images/videos/447/background.png"
  logoUrl="/images/logo.png"
  contentLogoUrl="/images/videos/contentLogos/code_unity_logo.png"
  vtuberImageUrl="/images/videos/vtubers/vtuber-2.0.png"
  portraitImageUrl="/images/videoThumbnail/headerBackground.png">
  <span slot="subtitle">打算從新專案開始出發</span>
  <span slot="title">Unity 開放世界專案 <span class="sub-font">#2</span></span>
</VideoThumbnail>