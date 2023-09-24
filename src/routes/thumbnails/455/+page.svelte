<script>
  import VideoThumbnail from '../../../components/videoThumbnail.svelte';
  import {data} from '../data';
</script>

<VideoThumbnail 
category="Code"
tagList={[data.tagList[1]]}
backgroundImageUrl="/images/videos/455/background.jpg"
logoUrl="/images/logo.png"
contentLogoUrl="/images/videos/contentLogos/code_chatgpt_logo.png"
vtuberImageUrl="/images/videos/vtubers/vtuber-1.0.png"
portraitImageUrl="/images/videoThumbnail/headerBackground.png"
volumeNumber=455>
<span slot="subtitle">來做些簡單的圖像、音樂和影片</span>
<span slot="title">ChatGPT 寫程式 <span class="sub-font">2023.08.08</span></span>
</VideoThumbnail>