<script lang="ts">
	import Calendar from '@event-calendar/core';
	import DayGrid from '@event-calendar/day-grid';
	import TimeGrid from '@event-calendar/time-grid';
	import Interaction from '@event-calendar/interaction';

	import '@event-calendar/core/index.css';

	let plugins = [TimeGrid, DayGrid, Interaction];
	let options = {
		view: 'timeGridWeek',
		height: 'inherit',
		headerToolbar: {
			start: 'prev,next, today',
			center: 'title',
			end: 'dayGridMonth,timeGridWeek,timeGridDay'
		},
		buttonText: function (texts: any) {
			texts.today = 'Today';
			texts.dayGridMonth = 'Month';
			texts.timeGridWeek = 'Week';
			texts.timeGridDay = 'Day';
			return texts;
		},
		scrollTime: '09:00:00',
		events: createEvents(),
		views: {
			timeGridWeek: { pointer: true, title: 'MMMM' },
			resourceTimeGridWeek: { pointer: true }
		},
		dayMaxEvents: true,
		nowIndicator: true,
		selectable: true
	};

	function createEvents() {
		let days = [];
		for (let i = 0; i < 7; ++i) {
			let day = new Date();
			let diff = i - day.getDay();
			day.setDate(day.getDate() + diff);
			days[i] = day.getFullYear() + '-' + _pad(day.getMonth() + 1) + '-' + _pad(day.getDate());
		}

		return [
			{ start: days[0] + ' 00:00', end: days[0] + ' 09:00', display: 'background' },
			{ start: days[1] + ' 12:00', end: days[1] + ' 14:00', display: 'background' },
			{ start: days[2] + ' 17:00', end: days[2] + ' 24:00', display: 'background' },
			{
				start: days[0] + ' 10:00',
				end: days[0] + ' 14:00',

				title: 'The calendar can display background and regular events',
				color: '#38bdf8'
			},
			{
				start: days[1] + ' 16:00',
				end: days[2] + ' 08:00',
				title: 'An event may span to another day',
				color: '#84cc16'
			},
			{
				start: days[2] + ' 09:00',
				end: days[2] + ' 13:00',
				title:
					'Events can be assigned to resources and the calendar has the resources view built-in',
				color: '#d946ef'
			},
			{
				start: days[3] + ' 14:00',
				end: days[3] + ' 20:00',
				title: '',
				color: '#cbd5e1'
			},
			{
				start: days[3] + ' 15:00',
				end: days[3] + ' 18:00',

				title: 'Overlapping events are positioned properly',
				color: '#a855f7'
			},
			{
				start: days[5] + ' 10:00',
				end: days[5] + ' 16:00',

				titleHTML: 'You have complete control over the <i><b>display</b></i> of events…',
				color: '#d946ef'
			},
			{
				start: days[5] + ' 14:00',
				end: days[5] + ' 19:00',
				title: '…and you can drag and drop the events!',
				color: '#a855f7'
			},
			{
				start: days[5] + ' 18:00',
				end: days[5] + ' 21:00',
				title: '',
				color: '#d946ef'
			},
			{
				start: days[1],
				end: days[3],
				title: 'All-day events can be displayed at the top',
				color: '#B29DD9',
				allDay: true
			}
		];
	}

	function _pad(num: number) {
		let norm = Math.floor(Math.abs(num));
		return (norm < 10 ? '0' : '') + norm;
	}
</script>

<Calendar {plugins} {options} />
