<script>
    import WeeklySchedule from "../../../components/weeklySchedule.svelte";
    import {data} from '../data';

    function addDays(date, days) {
        var newDate = new Date(date.valueOf());
        newDate.setDate(newDate.getDate() + days);
        return newDate;
    }

    const startDate = Date.parse("2023-06-19");
    const items = [
        {
            date: startDate,
            time: "21:30",
            name: `寶可夢 朱 <span class="text-2xl">#9</span>`,
            category: "Game",
            tags: [data.tagList[0]] 
        },
        {
            date: addDays(startDate, 1),
            time: "21:30",
            name: `嘗試使用 Unity 製作動作遊戲 <span class="text-2xl">#5</span>`,
            category: "Code",
            tags: [data.tagList[1]] 
        },
        {
            date: addDays(startDate, 2),
            time: "",
            name: `休息日`,
            category: "Null",
            tags: [] 
        },
        {
            date: addDays(startDate, 3),
            time: "",
            name: `可能突發`,
            category: "",
            tags: [] 
        },
        {
            date: addDays(startDate, 4),
            time: "",
            name: `休息日`,
            category: "Null",
            tags: [] 
        },
        {
            date: addDays(startDate, 5),
            time: "",
            name: `可能突發`,
            category: "",
            tags: [] 
        },
        {
            date: addDays(startDate, 6),
            time: "",
            name: `休息日`,
            category: "Null",
            tags: [] 
        },
    ];

    const cover = {
        artist: "猫島羽依 (@NekosimaYui)",
        imageUrl: "/images/schedule/100/cover.png"
    };
</script>

<WeeklySchedule items={items} cover={cover} weekNumber=100></WeeklySchedule>