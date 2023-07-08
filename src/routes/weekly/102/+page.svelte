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

    const startDate = Date.parse("2023-07-03");
    const items = [
        {
            date: startDate,
            time: "晚上",
            name: `Sonic Origins Plus <span class="text-2xl">#3</span>`,
            category: "Game",
            tags: [data.tagList[0]] 
        },
        {
            date: addDays(startDate, 1),
            time: "晚上",
            name: `LeetCode <span class="text-2xl">#17</span>`,
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
            time: "晚上",
            name: `薩爾達傳說 曠野之息 <span class="text-2xl">#4</span>`,
            category: "Game",
            tags: [data.tagList[0]] 
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
            name: `POPS & ANIME 歌回 <span class="text-2xl">${formatDate(addDays(startDate, 5))}</span>`,
            category: "Sing",
            tags: [data.tagList[2]] 
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

<WeeklySchedule items={items} cover={cover} weekNumber=102></WeeklySchedule>