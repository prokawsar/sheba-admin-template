<script>
	import Card from '$lib/components/card.svelte';
	import CardImage from '$lib/components/cardImage.svelte';
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
			<div class="md:w-1/2 md:flex-none lg:w-2/3">
				<Table />
			</div>
			<div class="w-full max-w-full md:w-1/2 lg:w-1/3 h-full">
				<Timeline />
			</div>
		</div>

		<div class="flex flex-col md:flex-row gap-3">
			<CardImage />
		</div>
	</div>
</div>
