<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Game"
    tagList={[data.tagList[0]]}
    backgroundImageUrl="/images/videos/510/background.jpeg"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/game_blue_protocol_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-4.0p.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground2.png">
    <span slot="subtitle">來玩玩台版的 Blue Protocol，順便試試看最近做的 VRoid 模型</span>
    <span slot="title">蔚藍色法則 <span class="sub-font">封測體驗</span></span>
</VideoThumbnail>