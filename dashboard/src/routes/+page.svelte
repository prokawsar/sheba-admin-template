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
	<div class="flex flex-col gap-3 mt-5">
		<div class="flex flex-row gap-3">
			<Card />
			<Card />
			<Card />
			<Card />
		</div>

		<div class="flex flex-row gap-3">
			<Table />
			<Timeline />
		</div>

		<div class="flex flex-wrap -mx-3">
			<CardImage />
		</div>
	</div>
</div>
