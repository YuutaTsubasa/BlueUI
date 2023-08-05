<script>
  import VideoThumbnail from '../../../components/videoThumbnail.svelte';
  import {data} from '../data';
</script>

<VideoThumbnail 
category="Talk"
tagList={[data.tagList[3]]}
backgroundImageUrl="/images/videos/440/background.png"
logoUrl="/images/logo.png"
contentLogoUrl="/images/videos/contentLogos/talk_logo.png"
vtuberImageUrl="/images/videos/vtubers/vtuber-2.0.png"
portraitImageUrl="/images/videoThumbnail/headerBackground.png"
volumeNumber=440>
<span slot="subtitle">好久沒來玩玩二選一的雜談主題了</span>
<span slot="title">二選一問題雜談 <span class="sub-font">2023.07.15</span></span>
</VideoThumbnail>