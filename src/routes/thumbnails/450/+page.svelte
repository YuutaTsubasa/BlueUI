<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
  category=""
  tagList={[data.tagList[3], data.tagList[2]]}
  backgroundImageUrl="/images/videos/450/background.jpg"
  logoUrl="/images/logo.png"
  contentLogoUrl=""
  vtuberImageUrl="/images/videos/vtubers/vtuber-2.0.png"
  portraitImageUrl="/images/videoThumbnail/headerBackground.png"
  volumeNumber=450>
  <span slot="subtitle">來一起來回顧這一年吧！</span>
  <span slot="title">二周年慶祝與回顧配信</span>
</VideoThumbnail>