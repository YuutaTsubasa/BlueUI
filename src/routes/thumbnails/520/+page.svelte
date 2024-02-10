<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Sing"
    tagList={[data.tagList[2]]}
    backgroundImageUrl="/images/videos/520/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/sing_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-4.0py.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground5.png">
    <span slot="subtitle">雖然早了兩天，但還是可以先來唱唱歌</span>
    <span slot="title">2023 聖誕節歌回</span>
</VideoThumbnail>