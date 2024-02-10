<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Game"
    tagList={[data.tagList[0]]}
    backgroundImageUrl="/images/videos/523/background.jpg"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/game_a_equals_b_logo.jpeg"
    vtuberImageUrl="/images/videos/vtubers/vtuber-3.0-c.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground6.png">
    <span slot="subtitle">趁新年假期，來玩玩好久沒開過的程式類型遊戲了！</span>
    <span slot="title">A=B</span>
</VideoThumbnail>