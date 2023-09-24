<script>
  import VideoThumbnail from '../../../components/videoThumbnail.svelte';
  import {data} from '../data';
  import { page } from '$app/stores';

  $: number = $page.url.pathname.split("/").findLast(value => value != "");
</script>

<VideoThumbnail 
category="Code"
tagList={[data.tagList[1]]}
backgroundImageUrl="/images/videos/461/background.png"
logoUrl="/images/logo.png"
contentLogoUrl=""
vtuberImageUrl=""
portraitImageUrl="/images/videoThumbnail/headerBackground.png"
volumeNumber={number}>
<span slot="subtitle">Midjourney, EasyVtuber, RVC, ChatGPT 等等套件的融合體</span>
<span slot="title">利用 AI 生成並驅動 Vtuber</span>
</VideoThumbnail>