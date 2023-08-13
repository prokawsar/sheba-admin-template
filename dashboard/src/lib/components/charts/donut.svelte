<script lang="ts">
	import ApexCharts from 'apexcharts';
	import { onMount } from 'svelte';

	var options = {
		series: [44, 55, 41, 17, 15],
		chart: {
			width: 380,
			type: 'donut'
		},
		plotOptions: {
			pie: {
				startAngle: -90,
				endAngle: 270
			}
		},
		dataLabels: {
			enabled: false
		},
		fill: {
			type: 'gradient'
		},
		legend: {
			formatter: function (val: string, opts: any) {
				return val + ' - ' + opts.w.globals.series[opts.seriesIndex];
			}
		},
		title: {
			text: 'Gradient Donut'
		},
		responsive: [
			{
				breakpoint: 480,
				options: {
					chart: {
						width: 200
					},
					legend: {
						position: 'bottom'
					}
				}
			}
		]
	};

	let tmr: any;

	onMount(() => {
		if (tmr) clearTimeout(tmr);
		tmr = setTimeout(() => {
			var chart = new ApexCharts(document.querySelector('#donut'), options);
			chart.render();
		}, 100);
	});
</script>

<div id="donut" />
