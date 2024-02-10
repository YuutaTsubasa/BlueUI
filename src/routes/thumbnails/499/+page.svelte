<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Mix"
    tagList={[data.tagList[2], data.tagList[3]]}
    backgroundImageUrl="/images/videos/431/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/sing_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-fix.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground2.png">
    <span slot="subtitle">聊聊天 & 唱唱歌</span>
    <span slot="title">2023 萬聖節雜談 & 歌回</span>
</VideoThumbnail>