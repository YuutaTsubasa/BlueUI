<script>
  import VideoThumbnail from '../../../components/videoThumbnail.svelte';
  import {data} from '../data';
</script>

<VideoThumbnail 
category="Game"
tagList={[data.tagList[0]]}
backgroundImageUrl="/images/videos/458/background.jpeg"
logoUrl="/images/logo.png"
contentLogoUrl="/images/videos/contentLogos/game_stephens_sausage_roll_logo.jpeg"
vtuberImageUrl="/images/videos/vtubers/vtuber-2.0.png"
portraitImageUrl="/images/videoThumbnail/headerBackground.png"
volumeNumber=458>
<span slot="subtitle">來烤香腸囉～感覺是個很燒腦的遊戲</span>
<span slot="title">Stephen's Sausage Roll <span class="sub-font">#1</span></span>
</VideoThumbnail>