<script>
	import '../app.css';
	import { page } from '$app/stores';
	import { browser } from '$app/environment';
	import posthog from 'posthog-js';
	import { onMount } from 'svelte';
	import Nav from '$lib/components/nav.svelte';

	onMount(() => {
		if (browser) {
			import('$lib/utils/tooltip');
		}
	});

	$: $page.url.pathname, browser && posthog.capture('$pageview', { layout: true });
</script>

<Nav />
<main class="md:ml-80 h-full relative">
	<slot />
</main>
