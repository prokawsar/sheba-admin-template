<script lang="ts">
	import { activeTab } from '$lib/stores/store';
	import { faIcons, type IconDefinition } from '@fortawesome/free-solid-svg-icons';
	import Fa from 'svelte-fa';

	export let link = '',
		text = '',
		onClick: Function = () => {},
		icon: IconDefinition = faIcons;
</script>

<a
	class:!shadow-lg={$activeTab == text.trim().toLocaleLowerCase().replace(/\s/g, '')}
	class="hover:shadow-md shadow-sm rounded-lg py-2 text-sm ease-nav-brand my-0 mx-4 flex items-center whitespace-nowrap px-4 transition-colors"
	href={link || ''}
	on:click={() => (onClick ? onClick() : null)}
>
	{#if icon}
		<div
			class="shadow-sm mr-2 flex h-8 w-8 items-center justify-center rounded-lg bg-white bg-center stroke-0 text-center xl:p-2"
		>
			<!-- <Customer /> -->
			<Fa {icon} />
		</div>
	{/if}
	<span class="ml-1 duration-300 opacity-100 pointer-events-none ease-soft">
		{text}
	</span>
</a>
