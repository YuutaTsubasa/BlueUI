<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Talk"
    tagList={[data.tagList[3]]}
    backgroundImageUrl="/images/videos/553/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/talk_davinci_resolve_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-c.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground6.png">
    <span slot="subtitle">聊聊頻道經營、聊聊企劃構思</span>
    <span slot="title">剪輯精華雜談 <span class="sub-font">2024.03.02</span></span>
</VideoThumbnail>