<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Mix"
    tagList={[data.tagList[1], data.tagList[3]]}
    backgroundImageUrl="/images/videos/431/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/talk_code_review_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-c.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground6.png">
    <span slot="subtitle">來看看自己寫的 Global Game Jam 的 MetaGame 部分</span>
    <span slot="title">Code Review 雜談 <span class="sub-font">#1</span></span>
</VideoThumbnail>