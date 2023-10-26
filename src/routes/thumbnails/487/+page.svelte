<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Code"
    tagList={[data.tagList[1]]}
    backgroundImageUrl="/images/videos/487/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/code_godot_engine_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-fix.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground2.png">
    <span slot="subtitle">繼續來做打字競速遊戲</span>
    <span slot="title">Godot Engine 探索 <span class="sub-font">#05</span></span>
</VideoThumbnail>