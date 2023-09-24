<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="3D"
    tagList={[data.tagList[5]]}
    backgroundImageUrl="/images/videos/475/background.jpeg"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/3d_vroid_studio_logo.webp"
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-b.PNG"
    portraitImageUrl="/images/videoThumbnail/headerBackground.png">
    <span slot="subtitle">難得來玩玩 VRoid Studio 吧！</span>
    <span slot="title">VRoid Studio <span class="sub-font">2023.09.09</span></span>
</VideoThumbnail>