<script>
  import VideoThumbnail from '../../../components/videoThumbnail.svelte';
  import {data} from '../data';
</script>

<VideoThumbnail 
category="Game"
tagList={[data.tagList[0]]}
backgroundImageUrl="/images/videos/434/background.png"
logoUrl="/images/logo.png"
contentLogoUrl="/images/videos/contentLogos/game_zelda_breath_of_wild_logo.png"
vtuberImageUrl="/images/videos/vtubers/vtuber-2.0.png"
portraitImageUrl="/images/videoThumbnail/headerBackground.png"
volumeNumber=434>
<span slot="subtitle">來到第二個村莊逛逛</span>
<span slot="title">薩爾達傳說 曠野之息 <span class="text-4xl">#4</span></span>
</VideoThumbnail>