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
vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-b.PNG"
portraitImageUrl="/images/videoThumbnail/headerBackground.png">
<span slot="subtitle">Problem 143. ~ Problem 145.</span>
<span slot="title">LeetCode <span class="sub-font">#23</span></span>
</VideoThumbnail>