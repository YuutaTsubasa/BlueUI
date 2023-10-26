<script>
    import VideoThumbnail from '../../../components/videoThumbnail.svelte';
    import {data} from '../data';
</script>

<VideoThumbnail 
    category="Game"
    tagList={[data.tagList[0]]}
    backgroundImageUrl="/images/videos/493/background.png"
    logoUrl="/images/logo.png"
    contentLogoUrl="/images/videos/contentLogos/game_party_animals_logo.webp"
    vtuberImageUrl="/images/videos/vtubers/vtuber-20231015.png"
    portraitImageUrl="/images/videoThumbnail/headerBackground2.png">
    <span slot="subtitle">猫島家大亂鬥 feat. 猫島家成員</span>
    <span slot="title">猛獸派對 Party Animals</span>
</VideoThumbnail>