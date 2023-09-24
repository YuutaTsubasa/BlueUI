<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
  category="Code"
  tagList={[data.tagList[1]]}
  backgroundImageUrl="/images/videos/468/background.png"
  logoUrl="/images/logo.png"
  contentLogoUrl="/images/videos/contentLogos/code_unity_logo.png"
  vtuberImageUrl="/images/videos/vtubers/vtuber-2.0.png"
  portraitImageUrl="/images/videoThumbnail/headerBackground.png">
  <span slot="subtitle">要來讓讀取的角色可以動來動去</span>
  <span slot="title">Unity 開放世界專案 <span class="sub-font">#3</span></span>
</VideoThumbnail>