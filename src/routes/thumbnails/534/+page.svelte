<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Code"
    tagList={[data.tagList[1]]}
    backgroundImageUrl="/images/videos/532/background.jpg"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/code_global_game_jam_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-global-game-jam.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground6.png">
    <span slot="subtitle">feat. 葵栗鹿鹿、Gairaku、陳旭元、花枝丸、緋千夜</span>
    <span slot="title">Global Game Jam 2024 <span class="sub-font">#3</span></span>
</VideoThumbnail>