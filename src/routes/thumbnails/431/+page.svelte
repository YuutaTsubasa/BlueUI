<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
  category="Talk"
  tagList={[data.tagList[3]]}
  backgroundImageUrl="/images/videos/431/background.png"
  logoUrl="/images/logo.png"
  contentLogoUrl="/images/videos/contentLogos/talk_logo.png"
  vtuberImageUrl="/images/videos/vtubers/vtuber-2.0.png"
  portraitImageUrl="/images/videoThumbnail/headerBackground.png"
  volumeNumber=431>
  <span slot="subtitle">來一起聊聊天吧！</span>
  <span slot="title">六月總結雜談 <span class="text-4xl">2023.07.01</span>
</VideoThumbnail>