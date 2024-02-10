<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Game"
    tagList={[data.tagList[0]]}
    backgroundImageUrl="/images/videos/539/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/game_atelier_resleriana_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-c.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground6.png">
    <span slot="subtitle">今天繼續來破主線，有空的話順便過個活動</span>
    <span slot="title" class="two-line-font">蕾斯萊莉婭娜的鍊金工房 <span class="sub-num-font">#2</span><br/><span class="sub-font">～忘卻的鍊金術與極夜的解放者～</span></span>
</VideoThumbnail>