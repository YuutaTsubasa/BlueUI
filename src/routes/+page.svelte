<script>
    import ProfileCard from "../components/profileCard.svelte";
    import VideoThumbnail from "../components/videoThumbnail.svelte";

    let communityList = [
        "twitter",
        "youtube",
        "facebook",
        "plurk",
        "instagram",
        "twitch",
        "discord"
    ];

    let thumbnailList = [
      "thumbnail2",
      "thumbnail3",
      "thumbnail4"
    ];
</script>

<ProfileCard 
    tagList={tagList}
    communityList={communityList}
    thumbnailList={thumbnailList}
    backgroundImageUrl="images/backgroundPerson.png"
    bottomBackgroundImageUrl="images/bottomBackground.png"
    portraitImageUrl="images/portrait.png"
    logoIconImageUrl="images/logoIcon.png">

    <span slot="title">盔甲正太程式 VTuber</span>
    <span slot="name">悠太翼</span>
    <span slot="id">@YuutaTsubasa</span>
    <span slot="logoImage" class="flex justify-center"><img src="images/logo.png" alt="Logo" class="w-[80%]"/></span>
    <span slot="videoAmount">483</span>
    <span slot="subscriberAmount">2450</span>
</ProfileCard>

<!-- <VideoThumbnail 
  category="Sing"
  tagList={[tagList[2]]}
  backgroundImageUrl="images/videoThumbnail/background-379.png"
  logoUrl="images/logo.png"
  contentLogoUrl="images/videoThumbnail/leftLogo.png"
  vtuberImageUrl="images/videoThumbnail/vtuber.png"
  portraitImageUrl="images/videoThumbnail/headerBackground.png"
  volumeNumber=418>
  <span slot="subtitle">終於要見到阿爾宙斯了！</span>
  <span slot="title">寶可夢傳說 阿爾宙斯 <span class="text-2xl">#18</span></span>
</VideoThumbnail> -->

<!-- <VideoThumbnail 
  category="Sing"
  tagList={[tagList[2]]}
  backgroundImageUrl="images/videoThumbnail/background-379.png"
  logoUrl="images/logo.png"
  contentLogoUrl="images/videoThumbnail/leftLogo-Sing.png"
  vtuberImageUrl="images/videoThumbnail/vtuber-1.0.png"
  portraitImageUrl="images/videoThumbnail/headerBackground.png"
  volumeNumber=423>
  <span slot="subtitle">來複習一些以前唱過的 V 家歌曲吧！</span>
  <span slot="title">VOCALOID 歌回 <span class="text-4xl">2023.06.18</span></span>
</VideoThumbnail> -->