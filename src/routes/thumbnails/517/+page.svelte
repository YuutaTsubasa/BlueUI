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
    vtuberImageUrl="/images/videos/vtubers/vtuber-4.0py.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground5.png">
    <span slot="subtitle">來跟大家聊聊自己整理的這篇文章吧！</span>
    <span slot="title">主題雜談 <span class="sub-font">「如何成為 Vtuber 的步驟與資源」</span></span>
</VideoThumbnail>