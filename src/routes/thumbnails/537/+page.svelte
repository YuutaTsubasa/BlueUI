<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
  category="Draw"
  tagList={[data.tagList[4]]}
  backgroundImageUrl="/images/videos/537/background.png"
  logoUrl="/images/logo.png"
  contentLogoUrl="/images/videos/contentLogos/draw_krita_logo.png"
  vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-c.png"
  portraitImageUrl="/images/videoThumbnail/headerBackground6.png">
  <span slot="subtitle">來完成 2024 年每月一次的畫圖目標吧！</span>
  <span slot="title">無限版本設定製作紀錄 <span class="sub-font">#2</span></span>
</VideoThumbnail>