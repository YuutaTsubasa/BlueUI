<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Game"
    tagList={[data.tagList[0]]}
    backgroundImageUrl="/images/videos/471/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/game_epic_seven_logo.png"
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-epic-seven.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground.png">
    <span slot="subtitle">來回鍋一下許久沒玩的手機遊戲了</span>
    <span slot="title">第七史詩 <span class="sub-font">#18</span></span>
</VideoThumbnail>