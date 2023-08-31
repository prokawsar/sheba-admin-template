<script lang="ts">
	import NavItem from '$lib/elements/navItem.svelte';
	import { activeTab } from '$lib/stores/store';
	import {
		faAlignCenter,
		faCalendarAlt,
		faCog,
		faDashboard,
		faDiamondTurnRight,
		faMoneyBill1Wave,
		faUser
	} from '@fortawesome/free-solid-svg-icons';
	import Fa from 'svelte-fa';
	import { slide } from 'svelte/transition';

	const groups: any = {
		showElements: false,
		showAuth: false,
		showPrice: false,
		showCharts: false,
		showGenpgaes: false
	};

	const collapseExpandMenu = (groupName: string = '') => {
		if (!groupName) return;
		groups[groupName] = !groups[groupName];

		for (const key in groups) {
			if (key !== groupName) {
				groups[key] = false;
			}
		}
	};
</script>

<aside
	transition:slide={{
		duration: 150,
		delay: 100,
		axis: 'x'
	}}
	class="max-w-xs shadow-xl bg-white w-full fixed pt-16 h-full flex flex-col justify-between z-20 inset-y-0"
>
	<div class="flex flex-col h-full">
		<!-- <div class="h-20">
			<i
				class="absolute top-0 right-0 hidden p-4 opacity-50 cursor-pointer fas fa-times text-slate-400 xl:hidden"
				aria-hidden="true"
			/>
			<a class="block px-8 py-6 m-0 text-sm whitespace-nowrap text-slate-700" href="/">
				<span class="ml-1 font-semibold transition-all duration-200 ease-nav-brand">
					Sheba Admin Dashboard
				</span>
			</a>
		</div> -->

		<!-- <hr
			class="h-px mt-0 bg-transparent bg-gradient-to-r from-transparent via-black/10 to-transparent"
		/> -->

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
					<NavItem
						text="Calendar"
						link="/calendar"
						icon={faCalendarAlt}
						onClick={() => ($activeTab = 'calendar')}
					/>
				</li>

				<li class="w-full">
					<!-- <NavItem
						text="Charts"
						icon={faChartLine}
						link="/charts"
						onClick={() => ($activeTab = 'charts')}
					/> -->

					<NavItem
						text="Charts"
						group
						bind:groupActive={groups['showCharts']}
						icon={faCog}
						onClick={() => {
							collapseExpandMenu('showCharts');
						}}
					/>

					{#if groups['showCharts']}
						<div
							transition:slide={{
								duration: 200,
								delay: 50,
								axis: 'y'
							}}
							class="flex flex-col"
						>
							<NavItem
								subItem
								link="/charts/chartjs"
								text="Chart.js"
								onClick={() => ($activeTab = 'chart.js')}
							/>
							<NavItem
								subItem
								link="/charts/apexchart"
								text="ApexChart"
								onClick={() => ($activeTab = 'apexchart')}
							/>
						</div>
					{/if}
				</li>

				<!-- <li class="w-full">
					<NavItem text="Tables" icon={faTable} onClick={() => ($activeTab = 'tables')} />
				</li> -->

				<li class="w-full">
					<NavItem
						text="UI Elements"
						group
						bind:groupActive={groups['showElements']}
						icon={faCog}
						onClick={() => {
							collapseExpandMenu('showElements');
						}}
					/>

					{#if groups['showElements']}
						<div
							transition:slide={{
								duration: 200,
								delay: 50,
								axis: 'y'
							}}
							class="flex flex-col"
						>
							<NavItem subItem link="/ui/alerts" text="Alerts" />
							<NavItem subItem link="/ui/buttons" text="Buttons" />
							<NavItem subItem link="/ui/datepicker" text="Datepicker" />
							<NavItem subItem link="/ui/modals" text="Modals" />
							<NavItem subItem link="/ui/panels" text="Panels" />
							<NavItem subItem link="/ui/tables" text="Tables" />
							<NavItem subItem link="/ui/tooltips" text="Tooltips" />
						</div>
					{/if}
				</li>

				<li class="w-full">
					<NavItem
						text="Pricing"
						group
						bind:groupActive={groups['showPrice']}
						icon={faMoneyBill1Wave}
						onClick={() => {
							collapseExpandMenu('showPrice');
						}}
					/>

					{#if groups['showPrice']}
						<div
							transition:slide={{
								duration: 200,
								delay: 50,
								axis: 'y'
							}}
							class="flex-col"
						>
							<NavItem subItem text="Column Pricing" />
							<NavItem subItem text="Table Pricing" />
						</div>
					{/if}
				</li>

				<li class="w-full">
					<NavItem
						text="Authentication"
						group
						bind:groupActive={groups['showAuth']}
						icon={faUser}
						onClick={() => {
							collapseExpandMenu('showAuth');
						}}
					/>

					{#if groups['showAuth']}
						<div
							transition:slide={{
								duration: 200,
								delay: 50,
								axis: 'y'
							}}
							class="flex-col"
						>
							<NavItem
								subItem
								text="Profile"
								link="/profile"
								onClick={() => ($activeTab = 'profile')}
							/>
							<NavItem
								subItem
								text="Sign In"
								link="/signin"
								onClick={() => ($activeTab = 'signin')}
							/>
							<NavItem
								subItem
								text="Sign Up"
								link="/signup"
								onClick={() => ($activeTab = 'signup')}
							/>
						</div>
					{/if}
				</li>

				<li class="w-full">
					<NavItem
						text="General Pages"
						group
						bind:groupActive={groups['showGenpgaes']}
						icon={faAlignCenter}
						onClick={() => {
							collapseExpandMenu('showGenpgaes');
						}}
					/>

					{#if groups['showGenpgaes']}
						<div
							transition:slide={{
								duration: 200,
								delay: 50,
								axis: 'y'
							}}
							class="flex-col"
						>
							<NavItem
								subItem
								text="Billing"
								link="/general-pages/billing"
								onClick={() => ($activeTab = 'billing')}
							/>
							<NavItem
								subItem
								text="FAQ"
								link="/general-pages/faq"
								onClick={() => ($activeTab = 'faq')}
							/>

							<NavItem
								subItem
								text="Error"
								link="/general-pages/error"
								onClick={() => ($activeTab = 'error')}
							/>
						</div>
					{/if}
				</li>
			</ul>
		</div>
	</div>
	<!-- <div
		class="after:opacity-65 after:bg-gradient-to-tl after:from-slate-600 after:to-slate-300 relative flex min-w-0 flex-col items-center break-words rounded-2xl border-0 border-solid border-blue-900 bg-white bg-clip-border shadow-none after:absolute after:top-0 after:bottom-0 after:left-0 after:z-10 after:block after:h-full after:w-full after:rounded-2xl after:content-['']"
	> -->
	<div class="mx-1">
		<div
			class="bg-gradient-to-tl from-slate-600 to-slate-300 relative z-20 flex-auto w-full p-4 text-left rounded-lg text-white"
		>
			<div
				class="flex items-center justify-center w-8 h-8 mb-4 text-center bg-white bg-center rounded-lg icon shadow-2xl"
			>
				<Fa icon={faDiamondTurnRight} class="text-gray-500" />
			</div>
			<div class="transition-all duration-200 ease-nav-brand">
				<h6 class="mb-0 text-white">Want to use on your project?</h6>
				<p class="mt-0 mb-4 text-xs font-semibold leading-tight">Please support with a coffee</p>
				<a
					href="/docs/"
					target="_blank"
					class="inline-block w-full px-8 py-2 mb-0 text-xs font-bold text-center text-black uppercase transition-all ease-in bg-white border-0 border-white rounded-lg shadow-soft-md bg-150 leading-pro hover:shadow-soft-2xl hover:scale-102"
				>
					Buy Now
				</a>
			</div>
		</div>
	</div>
	<!-- </div> -->
</aside>