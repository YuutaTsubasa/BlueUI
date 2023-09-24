<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
  category="Draw"
  tagList={[data.tagList[4]]}
  backgroundImageUrl="/images/videos/465/background.png"
  logoUrl="/images/logo.png"
  contentLogoUrl="/images/videos/contentLogos/draw_krita_logo.png"
  vtuberImageUrl="/images/videos/vtubers/vtuber-2.0.png"
  portraitImageUrl="/images/videoThumbnail/headerBackground.png">
  <span slot="subtitle">先從嘗試繪製設定開始吧！</span>
  <span slot="title">無限版本設定製作紀錄 <span class="sub-font">#1</span></span>
</VideoThumbnail>