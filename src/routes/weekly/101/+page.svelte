<script>
    import WeeklySchedule from "../../../components/weeklySchedule.svelte";
    import {data} from '../data';

    function addDays(date, days) {
        var newDate = new Date(date.valueOf());
        newDate.setDate(newDate.getDate() + days);
        return newDate;
    }

    const startDate = Date.parse("2023-06-26");
    const items = [
        {
            date: startDate,
            time: "21:30",
            name: `Sonic Origins Plus <span class="text-2xl">#2</span>`,
            category: "Game",
            tags: [data.tagList[0]] 
        },
        {
            date: addDays(startDate, 1),
            time: "21:30",
            name: `直播聊天室擷取程式 <span class="text-2xl">#7</span>`,
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
            time: "21:30",
            name: `LeetCode <span class="text-2xl">#16</span>`,
            category: "Code",
            tags: [data.tagList[1]] 
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
            time: "21:30",
            name: `六月總結雜談 <span class="text-2xl">2023.07.01</span>`,
            category: "Talk",
            tags: [data.tagList[3]] 
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

<WeeklySchedule items={items} cover={cover} weekNumber=101></WeeklySchedule>