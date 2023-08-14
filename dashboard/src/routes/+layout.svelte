<script>
	import '../app.css';
	import { page } from '$app/stores';
	import { browser } from '$app/environment';
	import posthog from 'posthog-js';
	import { onMount } from 'svelte';
	import NavSide from '$lib/components/navSide.svelte';
	import Footer from '$lib/components/footer.svelte';
	import NavTop from '$lib/components/navTop.svelte';
	import SettingsSide from '$lib/components/settingsSide.svelte';

	onMount(() => {
		if (browser) {
			import('$lib/utils/tooltip');
		}
	});

	$: $page.url.pathname, browser && posthog.capture('$pageview', { layout: true });

	let showSideNav = true,
		showSideSettings = false;
</script>

<div class="flex flex-col w-full">
	<!-- <NavTop /> -->
	<div class="w-full z-50">
		<NavTop bind:showSideNav bind:showSideSettings />
	</div>
	<div class=" h-full pt-16">
		{#if showSideNav}
			<NavSide />
		{/if}
		<main
			class="{showSideNav
				? 'lg:pl-80'
				: ''} bg-gray-50 h-fullrelative transition-all duration-150 delay-75"
		>
			<!-- <div class="mx-4">
				<NavTop />
			</div> -->
			<slot />
			<Footer />
		</main>
		{#if showSideSettings}
			<SettingsSide bind:showSideSettings />
		{/if}
	</div>
</div>
