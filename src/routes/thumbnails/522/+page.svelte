<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Mix"
    tagList={[data.tagList[3], data.tagList[2]]}
    backgroundImageUrl="/images/videos/522/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl=""
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-c.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground6.png">
    <span slot="subtitle">兼 2023 年度回顧雜談</span>
    <span slot="title">3.0 Live2D 初登場</span>
</VideoThumbnail>