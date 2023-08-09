<script>
	import Card from '$lib/components/card.svelte';
	import NavTop from '$lib/components/navTop.svelte';
	import Table from '$lib/components/table.svelte';
	import { i, languages, switchLanguage } from '@inlang/sdk-js';
</script>

<svelte:head>
	<title>Dashboard starter</title>
</svelte:head>

<div class="mx-4">
	<NavTop />

	<div class="flex flex-col gap-3 mt-5">
		<div class="flex flex-row">
			<Card />
			<Card />
			<Card />
			<Card />
		</div>

		<Table />
	</div>
</div>
