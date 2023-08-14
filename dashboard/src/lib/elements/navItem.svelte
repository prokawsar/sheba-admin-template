<script lang="ts">
	import { activeTab } from '$lib/stores/store';
	import {
		faChevronDown,
		faChevronUp,
		type IconDefinition
	} from '@fortawesome/free-solid-svg-icons';
	import Fa from 'svelte-fa';

	export let link = '',
		classes = '',
		text = '',
		group = false,
		groupActive = false,
		subItem = false,
		onClick: Function = () => {},
		icon: IconDefinition = {
			iconName: 'hooli',
			icon: [0, 0, ['0', '0'], '0', ''],
			prefix: 'far'
		};

	let hover = false;
	$: activeMenu = $activeTab == text.trim().toLocaleLowerCase().replace(/\s/g, '');
</script>

<a
	on:mouseenter={() => (hover = true)}
	on:mouseleave={() => (hover = false)}
	class:!shadow-md={groupActive}
	class:!shadow-lg={activeMenu}
	class="hover:shadow-md shadow-sm rounded-sm py-2 text-sm my-0 mx-4 flex items-center whitespace-nowrap px-4 transition-colors
	 {classes}"
	href={link || ''}
	on:click={() => (onClick ? onClick() : null)}
>
	{#if icon.iconName != 'hooli'}
		<div
			class="shadow-sm mr-2 flex h-8 w-8 items-center justify-center rounded-md bg-white text-center xl:p-2"
		>
			<Fa {icon} class="text-gray-500 {hover || activeMenu ? '!text-black' : ''}" />
		</div>
	{/if}
	<span
		class="ml-1 text-gray-700 duration-300 pointer-events-none {hover || activeMenu
			? '!text-black'
			: ''} {subItem ? 'pl-12 text-slate-500' : ''}"
	>
		{text}
	</span>
	<span class="grow" />
	{#if group}
		<Fa icon={groupActive ? faChevronUp : faChevronDown} size=".8x" />
	{/if}
</a>
