<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Game"
    tagList={[data.tagList[0]]}
    backgroundImageUrl="/images/videos/482/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/game_armored_core_vi_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-b.PNG"
    portraitImageUrl="/images/videoThumbnail/headerBackground.png">
    <span slot="subtitle">Armored Core VI: Fires of Rubicon</span>
    <span slot="title">機戰傭兵VI 境界天火 <span class="sub-font">#5</span></span>
</VideoThumbnail>