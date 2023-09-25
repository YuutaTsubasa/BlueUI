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

    const startDate = Date.parse("2023-09-25");
    const items = [
        {
            date: startDate,
            time: "晚上",
            name: `機戰傭兵VI 境界天火`,
            category: "Game",
            tags: [data.tagList[0]] 
        },
        {
            date: addDays(startDate, 1),
            time: "晚上",
            name: `用 Godot Engine 製作打字競速遊戲`,
            category: "Code",
            tags: [data.tagList[1]] 
        },
        {
            date: addDays(startDate, 2),
            time: "",
            name: `第一屆 VRAST! 大對決：決賽`,
            category: "Video",
            tags: [data.tagList[5]] 
        },
        {
            date: addDays(startDate, 3),
            time: "晚上",
            name: `Sonic Frontiers DLC`,
            category: "Game",
            tags: [data.tagList[0]] 
        },
        {
            date: addDays(startDate, 4),
            time: "",
            name: `VARK SHORTS 影片 #3`,
            category: "Video",
            tags: [data.tagList[5]] 
        },
        {
            date: addDays(startDate, 5),
            time: "晚上",
            name: `(視情況開) Godot 重做中秋節烤肉遊戲？`,
            category: "Code",
            tags: [data.tagList[1]] 
        },
        {
            date: addDays(startDate, 6),
            time: "22:30",
            name: `(視情況開) 同步視聽 SICP 公開課 #5`,
            category: "Code",
            tags: [data.tagList[1]] 
        },
    ];

    const cover = {
        artist: "",
        imageUrl: "/images/schedule/114/cover.png"
    };
</script>

<WeeklySchedule items={items} cover={cover}></WeeklySchedule>