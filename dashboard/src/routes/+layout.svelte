<script>
	import '../app.css';
	import { page } from '$app/stores';
	import { browser } from '$app/environment';
	import posthog from 'posthog-js';
	import { onMount } from 'svelte';
	import Nav from '$lib/components/nav.svelte';
	import Footer from '$lib/components/footer.svelte';
	import NavTop from '$lib/components/navTop.svelte';

	onMount(() => {
		if (browser) {
			import('$lib/utils/tooltip');
		}
	});

	$: $page.url.pathname, browser && posthog.capture('$pageview', { layout: true });
</script>

<Nav />
<main class="md:ml-80 h-full relative">
	<div class="mx-4">
		<NavTop />
	</div>
	<slot />
	<Footer />
</main>
