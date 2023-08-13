<script>
	import Doughnut from '$lib/components/charts/doughnut.svelte';
	import Line from '$lib/components/charts/line.svelte';
</script>

<svelte:head>
	<title>Dashboard starter</title>
</svelte:head>

<div class="mx-4">
	<div class="flex flex-col gap-5 pt-5">
		<div class="flex flex-row gap-3 h-96">
			<div class="flex-1 bg-white shadow-lg rounded-md p-2">
				<Line />
			</div>
		</div>
		<div class="flex flex-row gap-3 h-96">
			<div class="flex-1 bg-white shadow-lg rounded-md">
				<Line datasetsConfig={{ fill: true }} />
			</div>
			<div class="flex-1 bg-white justify-center items-center flex shadow-lg rounded-md">
				<Doughnut />
			</div>
		</div>
	</div>
</div>
