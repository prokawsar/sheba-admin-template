<script>
	import Scatter from '$lib/components/charts/scatter.svelte';
	import Donut from '$lib/components/charts/donut.svelte';
	import Spline from '$lib/components/charts/spline.svelte';
	import Xaxis from '$lib/components/charts/xaxis.svelte';
</script>

<svelte:head>
	<title>Charts | ApexChart</title>
</svelte:head>

<div class="mx-4">
	<div class="flex flex-col gap-5 mt-5">
		<div class="flex h-96">
			<div class="flex-1 shadow-lg rounded-md p-2">
				<Spline />
			</div>
		</div>

		<div class="flex h-96">
			<div class="flex-1 shadow-lg rounded-md p-2">
				<Xaxis />
			</div>
		</div>

		<div class="flex flex-row gap-3 h-96">
			<div class="flex-1 shadow-lg rounded-md">
				<Scatter />
			</div>
			<div class="flex-1 justify-center items-center flex shadow-lg rounded-md">
				<Donut />
			</div>
		</div>
	</div>
</div>
