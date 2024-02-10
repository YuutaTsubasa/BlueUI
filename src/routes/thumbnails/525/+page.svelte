<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Talk"
    tagList={[data.tagList[3]]}
    backgroundImageUrl="/images/videos/525/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/talk_inochi2d_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-c.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground6.png">
    <span slot="subtitle">從來沒玩過 Inochi2D，來使用看看</span>
    <span slot="title">Inochi2D 測試雜談</span>
</VideoThumbnail>