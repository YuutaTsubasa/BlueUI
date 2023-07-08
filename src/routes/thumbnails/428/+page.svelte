<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
  category="Code"
  tagList={[data.tagList[1]]}
  backgroundImageUrl="/images/videos/428/background.png"
  logoUrl="/images/logo.png"
  contentLogoUrl="/images/videos/contentLogos/code_twitch_logo.png"
  vtuberImageUrl="/images/videos/vtubers/vtuber-1.0.png"
  portraitImageUrl="/images/videoThumbnail/headerBackground.png"
  volumeNumber=428>
  <span slot="subtitle">複習之前做的東西，並且擷取 Twitch 的聊天室</span>
  <span slot="title">直播聊天室擷取程式 <span class="text-4xl">#7</span></span>
</VideoThumbnail>