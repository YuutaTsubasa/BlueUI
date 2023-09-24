<script>
    import WeeklySchedule from "../../../components/weeklySchedule.svelte";
    import {data} from '../data';

    function addDays(date, days) {
        var newDate = new Date(date.valueOf());
        newDate.setDate(newDate.getDate() + days);
        return newDate;
    }

    function formatDate(date) {
        const d = new Date(date);
        let month = '' + (d.getMonth() + 1),
            day = '' + d.getDate(),
            year = d.getFullYear();

        if (month.length < 2) 
            month = '0' + month;
        if (day.length < 2) 
            day = '0' + day;

        return [year, month, day].join('.');
    }

    const startDate = Date.parse("2023-09-04");
    const items = [
        {
            date: startDate,
            time: "晚上",
            name: `機戰傭兵VI 境界天火 <span class="text-2xl">#3</span>`,
            category: "Game",
            tags: [data.tagList[0]] 
        },
        {
            date: addDays(startDate, 1),
            time: "晚上",
            name: `<主題為會員投票決定>`,
            category: "Code",
            tags: [data.tagList[1]] 
        },
        {
            date: addDays(startDate, 2),
            time: "",
            name: `VARK SHORTS 影片 #1`,
            category: "Video",
            tags: [data.tagList[5]] 
        },
        {
            date: addDays(startDate, 3),
            time: "晚上",
            name: `始世樂土 Craftopia <span class="text-2xl">#3</span>`,
            category: "Game",
            tags: [data.tagList[0]] 
        },
        {
            date: addDays(startDate, 4),
            time: "",
            name: `VARK SHORTS 影片 #2`,
            category: "Video",
            tags: [data.tagList[5]] 
        },
        {
            date: addDays(startDate, 5),
            time: "晚上",
            name: `第七史詩 #19 / 3.0 亮相後第一次雜談`,
            category: "Mix",
            tags: [data.tagList[0], data.tagList[3]] 
        },
        {
            date: addDays(startDate, 6),
            time: "22:30",
            name: `同步視聽 SICP 公開課 #3`,
            category: "Code",
            tags: [data.tagList[1]] 
        },
    ];

    const cover = {
        artist: "猫島羽依 (@NekosimaYui)",
        imageUrl: "/images/schedule/100/cover.png"
    };
</script>

<WeeklySchedule items={items} cover={cover}></WeeklySchedule>