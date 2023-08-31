<script>
	import Card from '$lib/components/card.svelte';
	import CardImage from '$lib/components/cardImage.svelte';
	import Line from '$lib/components/charts/line.svelte';
	import Scatter from '$lib/components/charts/scatter.svelte';
	import NavTop from '$lib/components/navTop.svelte';
	import Table from '$lib/components/table.svelte';
	import Timeline from '$lib/components/timeline.svelte';
	import { i, languages, switchLanguage } from '@inlang/sdk-js';
</script>

<svelte:head>
	<title>Dashboard starter</title>
</svelte:head>

<div class="mx-4">
	<div class="flex flex-col gap-3">
		<div class="grid grid-cols-2 md:flex md:flex-row gap-3">
			<Card />
			<Card />
			<Card />
			<Card />
		</div>

		<div class="flex flex-col md:flex-row gap-3">
			<!-- <Table /> -->
			<div
				class="w-full bg-white shadow-xl rounded-2xl max-w-full mt-0 md:w-1/2 md:flex-none lg:w-2/3 lg:flex-none"
			>
				<Scatter />
			</div>
			<Timeline />
		</div>

		<div class="flex flex-col md:flex-row gap-3">
			<CardImage />
		</div>
	</div>
</div>
