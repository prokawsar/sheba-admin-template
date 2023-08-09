<script>
	import Card from '$lib/components/card.svelte';
	import NavTop from '$lib/components/navTop.svelte';
	import { i, languages, switchLanguage } from '@inlang/sdk-js';
</script>

<svelte:head>
	<title>Dashboard starter</title>
</svelte:head>

<div class="mx-4">
	<NavTop />

	<div class="flex flex-row">
		<Card />
		<Card />
		<Card />
		<Card />
	</div>
</div>
