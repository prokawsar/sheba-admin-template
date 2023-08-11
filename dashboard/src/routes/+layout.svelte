<script>
	import '../app.css';
	import { page } from '$app/stores';
	import { browser } from '$app/environment';
	import posthog from 'posthog-js';
	import { onMount } from 'svelte';
	import Nav from '$lib/components/nav.svelte';
	import Footer from '$lib/components/footer.svelte';
	import NavTop from '$lib/components/navTop.svelte';
	import { slide } from 'svelte/transition';

	onMount(() => {
		if (browser) {
			import('$lib/utils/tooltip');
		}
	});

	$: $page.url.pathname, browser && posthog.capture('$pageview', { layout: true });

	let showSideNav = true;
</script>

<div class="flex flex-col w-full px-1">
	<!-- <NavTop /> -->
	<div class="w-full z-50">
		<NavTop bind:show={showSideNav} />
	</div>
	<div class=" h-full pt-16">
		{#if showSideNav}
			<Nav />
		{/if}
		<main
			class="h-full relative transition transform duration-700 delay-700 ease-linear"
			class:pl-80={showSideNav}
		>
			<!-- <div class="mx-4">
				<NavTop />
			</div> -->
			<slot />
			<Footer />
		</main>
	</div>
</div>
