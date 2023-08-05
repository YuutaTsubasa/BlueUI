<script>
  import VideoThumbnail from '../../../components/videoThumbnail.svelte';
  import {data} from '../data';
</script>

<VideoThumbnail 
category="Code"
tagList={[data.tagList[1]]}
backgroundImageUrl="/images/videos/429/background.png"
logoUrl="/images/logo.png"
contentLogoUrl="/images/videos/contentLogos/code_leetcode_logo.png"
vtuberImageUrl="/images/videos/vtubers/vtuber-2.0.png"
portraitImageUrl="/images/videoThumbnail/headerBackground.png"
volumeNumber=438>
<span slot="subtitle">Problem 116. ~ Problem 123.</span>
<span slot="title">LeetCode <span class="sub-font">#18</span></span>
</VideoThumbnail>