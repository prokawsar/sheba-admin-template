<script>
	import NavItem from '$lib/elements/navItem.svelte';
	import { activeTab } from '$lib/stores/store';
	import {
		faCog,
		faDashboard,
		faMultiply,
		faTable,
		faUser
	} from '@fortawesome/free-solid-svg-icons';
	import Fa from 'svelte-fa';
	import { slide } from 'svelte/transition';

	export let showSideSettings = false;

	let showElements = false;
</script>

<aside
	transition:slide={{
		duration: 150,
		delay: 100,
		axis: 'x'
	}}
	class="right-0 max-w-xs shadow-xl bg-slate-50 w-full fixed h-full flex flex-col justify-between z-50 inset-y-0"
>
	<div class="flex flex-col h-full">
		<div class="h-10 relative">
			<button
				class="absolute flex items-center justify-center hover:bg-gray-200/60 h-6 w-6 rounded-full left-2 top-3"
				on:click={() => (showSideSettings = false)}
			>
				<Fa icon={faMultiply} class="" />
			</button>
		</div>

		<div class="h-20">
			<div class="block px-8 py-6 m-0 text-sm whitespace-nowrap text-slate-700">
				<span class="ml-1 font-semibold text-xl transition-all duration-200 ease-nav-brand">
					Sheba Admin Configuration
				</span>
			</div>
		</div>

		<hr
			class="h-px mt-0 bg-transparent bg-gradient-to-r from-transparent via-black/10 to-transparent"
		/>

		<div class="items-center h-full block w-auto overflow-auto grow basis-full">
			<ul class="flex flex-col pl-0 mb-0">
				<li class="w-full">
					<NavItem
						text="Dashboard"
						icon={faDashboard}
						link="/"
						onClick={() => ($activeTab = 'dashboard')}
					/>
				</li>

				<li class="w-full">
					<NavItem text="Tables" icon={faTable} onClick={() => ($activeTab = 'tables')} />
				</li>

				<li class="w-full">
					<NavItem
						text="UI Elements"
						icon={faCog}
						onClick={() => {
							(showElements = !showElements), ($activeTab = 'uielements');
						}}
					/>
				</li>
			</ul>
		</div>
	</div>
</aside>
