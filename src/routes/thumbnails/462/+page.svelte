<script>
  import VideoThumbnail from '../../../components/videoThumbnail.svelte';
  import {data} from '../data';
  import { page } from '$app/stores';

  $: number = $page.url.pathname.split("/").findLast(value => value != "");
</script>

<VideoThumbnail 
category="Game"
tagList={[data.tagList[0]]}
backgroundImageUrl="/images/videos/462/background.png"
logoUrl="/images/logo.png"
contentLogoUrl="/images/videos/contentLogos/game_rhythm_sprout_logo.webp"
vtuberImageUrl="/images/videos/vtubers/vtuber-2.0.png"
portraitImageUrl="/images/videoThumbnail/headerBackground.png"
volumeNumber={number}>
<span slot="subtitle">繼續來玩這個比太鼓之達人還嚴格的節奏遊戲！</span>
<span slot="title">Rhythm Sprout <span class="sub-font">#2</span></span>
</VideoThumbnail>