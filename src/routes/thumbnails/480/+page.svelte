<script>
  import VideoThumbnail from '../../../components/videoThumbnail.svelte';
  import {data} from '../data';
</script>

<VideoThumbnail 
category="Mix"
tagList={[data.tagList[0], data.tagList[2]]}
backgroundImageUrl="/images/videos/480/background.jpeg"
logoUrl="/images/logo.png"
contentLogoUrl="/images/videos/contentLogos/game_bus_simulator_21_logo.png"
vtuberImageUrl="/images/videos/vtubers/vtuber-3.0x-0916.png"
portraitImageUrl="/images/videoThumbnail/headerBackground.png">
<span slot="subtitle">開開巴士、唱唱歌、用用調整後的模型</span>
<span slot="title">Bus Simulator 21 <span class="sub-font">兼歌回</span></span>
</VideoThumbnail>