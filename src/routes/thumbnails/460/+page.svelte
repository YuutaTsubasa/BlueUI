<script>
  import VideoThumbnail from '../../../components/videoThumbnail.svelte';
  import {data} from '../data';
  import { page } from '$app/stores';
  
  $: number = $page.url.pathname.split("/").findLast(value => value != "");
</script>

<VideoThumbnail 
category="Code"
tagList={[data.tagList[1]]}
backgroundImageUrl="/images/videos/460/background.png"
logoUrl="/images/logo.png"
contentLogoUrl=""
vtuberImageUrl="/images/videos/vtubers/vtuber-2.0.png"
portraitImageUrl="/images/videoThumbnail/headerBackground.png"
volumeNumber={number}>
<span slot="subtitle">可以參考 Material UI 來做一套自己的設計</span>
<span slot="title">來嘗試寫一套 UI 吧！</span>
</VideoThumbnail>