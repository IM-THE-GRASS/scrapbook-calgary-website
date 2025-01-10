<script>
    import { Label } from "$lib/components/ui/label";

    import {
        Timeline,
        TimelineItem,
        TimelineSeparator,
        TimelineDot,
        TimelineConnector,
        TimelineContent,
        TimelineOppositeContent
    } from 'svelte-vertical-timeline';

    const Mar15events = [
        { title: 'Doors open', time: '8:30 am' },
        { title: 'Opening ceremony', time: '9:00 am' },
        { title: 'Code', time: '09:30 pm' },
        { title: 'Lunch', time: '12:00 pm' },
        { title: 'Code', time: '01:00 pm' },
        { title: 'Dinner', time: '06:00 pm' },
        { title: 'Code', time: '07:00 pm' },
        { title: 'Sleep', time: 'NEVER' },
    ];
</script>

<Timeline position="alternate">
    <Label class="title text-3xl m-0 font-bold text-nowrap">Saturday, March 15</Label>
	{#each Mar15events as event}
		<TimelineItem>
			<TimelineOppositeContent slot="opposite-content">
				
                <Label class="label text-2xl m-0 font-bold">{event.time}</Label>
			</TimelineOppositeContent>
			<TimelineSeparator>
				<TimelineDot style="background-color:white"/>
				<TimelineConnector />
			</TimelineSeparator>
			<TimelineContent>
				<Label class="title text-2xl m-0 font-bold">{event.title}</Label>
			</TimelineContent>
		</TimelineItem>
	{/each}
</Timeline>