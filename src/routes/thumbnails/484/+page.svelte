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
    vtuberImageUrl="/images/videos/vtubers/vtuber-custom-half.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground.png">
    <span slot="subtitle">從用向量繪圖畫線到一般繪圖上色，最後套 Live2D 模板的成果展示</span>
    <span slot="title">自繪自製 Live2D 成果雜談</span>
</VideoThumbnail>