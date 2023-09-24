<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Game"
    tagList={[data.tagList[0]]}
    backgroundImageUrl="/images/videos/470/background.jpeg"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/game_samba_logo.webp"
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground.png">
    <span slot="subtitle">來亮相 3.0 囉！</span>
    <span slot="title">Samba de Amigo <span class="sub-font">歡樂搖搖派對</span></span>
</VideoThumbnail>