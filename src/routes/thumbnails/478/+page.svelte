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
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-b.PNG"
    portraitImageUrl="/images/videoThumbnail/headerBackground.png">
    <span slot="subtitle">晚回家只能跟大家聊聊天了QQ</span>
    <span slot="title">工作雜談 <span class="sub-font">2023.09.12</span></span>
</VideoThumbnail>