<script>
	import Box_3d from '$lib/icons/box-3d.svelte';
	import Credit from '$lib/icons/credit.svelte';
	import Customer from '$lib/icons/customer.svelte';
	import Document from '$lib/icons/document.svelte';
	import Office from '$lib/icons/office.svelte';
	import Settings from '$lib/icons/settings.svelte';
	import Shop from '$lib/icons/shop.svelte';
	import Spaceship from '$lib/icons/spaceship.svelte';
	import { activeTab } from '$lib/stores/store';
	import { faDiamondTurnRight } from '@fortawesome/free-solid-svg-icons';
	import Fa from 'svelte-fa';
</script>

<aside
	class="max-w-xs bg-slate-100/20 w-full fixed pt-20 h-full flex flex-col justify-between z-10 inset-y-0"
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

		<hr
			class="h-px mt-0 bg-transparent bg-gradient-to-r from-transparent via-black/10 to-transparent"
		/>

		<div class="items-center h-full block w-auto overflow-auto grow basis-full">
			<ul class="flex flex-col pl-0 mb-0">
				<li class="w-full">
					<a
						class:shadow-xl={$activeTab == '/'}
						class="py-2 text-sm ease-nav-brand my-0 mx-4 flex items-center whitespace-nowrap rounded-lg bg-white px-4 font-semibold text-slate-700 transition-colors"
						href="/"
						on:click={() => ($activeTab = '/')}
					>
						<div
							class="bg-gradient-to-tl from-purple-700 to-pink-500 shadow-xl mr-2 flex h-8 w-8 items-center justify-center rounded-lg bg-white bg-center stroke-0 text-center xl:p-2"
						>
							<Shop />
						</div>
						<span class="ml-1 duration-300 opacity-100 pointer-events-none ease-soft">
							Dashboard
						</span>
					</a>
				</li>

				<li class="w-full">
					<a
						class="hover:shadow-xl rounded-lg py-2 text-sm ease-nav-brand my-0 mx-4 flex items-center whitespace-nowrap px-4 transition-colors"
						href="./pages/tables.html"
					>
						<div
							class="shadow-xl mr-2 flex h-8 w-8 items-center justify-center rounded-lg bg-white bg-center stroke-0 text-center xl:p-2"
						>
							<Office />
						</div>
						<span class="ml-1 duration-300 opacity-100 pointer-events-none ease-soft">
							Tables
						</span>
					</a>
				</li>

				<li class="w-full">
					<a
						class:shadow-xl={$activeTab == 'billing'}
						class="hover:shadow-xl rounded-lg py-2 text-sm ease-nav-brand my-0 mx-4 flex items-center whitespace-nowrap px-4 transition-colors"
						href="/billing"
						on:click={() => ($activeTab = 'billing')}
					>
						<div
							class="shadow-xl mr-2 flex h-8 w-8 items-center justify-center rounded-lg bg-white bg-center fill-current stroke-0 text-center xl:p-2"
						>
							<Credit />
						</div>
						<span class="ml-1 duration-300 opacity-100 pointer-events-none ease-soft">
							Billing
						</span>
					</a>
				</li>

				<li class="w-full">
					<a
						class="hover:shadow-xl rounded-lg py-2 text-sm ease-nav-brand my-0 mx-4 flex items-center whitespace-nowrap px-4 transition-colors"
						href="./pages/rtl.html"
					>
						<div
							class="shadow-xl mr-2 flex h-8 w-8 items-center justify-center rounded-lg bg-white bg-center stroke-0 text-center xl:p-2"
						>
							<Settings />
						</div>
						<span class="ml-1 duration-300 opacity-100 pointer-events-none ease-soft"> RTL </span>
					</a>
				</li>

				<li class="w-full mt-4">
					<h6 class="pl-6 ml-2 text-xs font-bold leading-tight uppercase opacity-60">
						Account pages
					</h6>
				</li>

				<li class="w-full">
					<a
						class="hover:shadow-xl rounded-lg py-2 text-sm ease-nav-brand my-0 mx-4 flex items-center whitespace-nowrap px-4 transition-colors"
						href="./pages/profile.html"
					>
						<div
							class="shadow-xl mr-2 flex h-8 w-8 items-center justify-center rounded-lg bg-white bg-center stroke-0 text-center xl:p-2"
						>
							<Customer />
						</div>
						<span class="ml-1 duration-300 opacity-100 pointer-events-none ease-soft">
							Profile
						</span>
					</a>
				</li>

				<li class=" w-full">
					<a
						class="hover:shadow-xl rounded-lg py-2 text-sm ease-nav-brand my-0 mx-4 flex items-center whitespace-nowrap px-4 transition-colors"
						href="signin"
					>
						<div
							class="shadow-xl mr-2 flex h-8 w-8 items-center justify-center rounded-lg bg-white bg-center stroke-0 text-center xl:p-2"
						>
							<Document />
						</div>
						<span class="ml-1 duration-300 opacity-100 pointer-events-none ease-soft">
							Sign In
						</span>
					</a>
				</li>

				<li class="w-full">
					<a
						class="hover:shadow-xl rounded-lg py-2 text-sm ease-nav-brand my-0 mx-4 flex items-center whitespace-nowrap px-4 transition-colors"
						href="/signup"
					>
						<div
							class="shadow-xl mr-2 flex h-8 w-8 items-center justify-center rounded-lg bg-white bg-center stroke-0 text-center xl:p-2"
						>
							<Spaceship />
						</div>
						<span class="ml-1 duration-300 opacity-100 pointer-events-none ease-soft">
							Sign Up
						</span>
					</a>
				</li>
			</ul>
		</div>
	</div>
	<div
		class="after:opacity-65 after:bg-gradient-to-tl after:from-slate-600 after:to-slate-300 relative flex min-w-0 flex-col items-center break-words rounded-2xl border-0 border-solid border-blue-900 bg-white bg-clip-border shadow-none after:absolute after:top-0 after:bottom-0 after:left-0 after:z-10 after:block after:h-full after:w-full after:rounded-2xl after:content-['']"
	>
		<div class="mb-7 absolute h-full w-full rounded-2xl bg-cover bg-center" />
		<div class="relative z-20 flex-auto w-full p-4 text-left text-white">
			<div
				class="flex items-center justify-center w-8 h-8 mb-4 text-center bg-white bg-center rounded-lg icon shadow-soft-2xl"
			>
				<!-- <i
					class="top-0 z-10 text-lg leading-none text-transparent ni ni-diamond bg-gradient-to-tl from-slate-600 to-slate-300 bg-clip-text opacity-80"
				/> -->
				<Fa icon={faDiamondTurnRight} class="text-gray-500" />
			</div>
			<div class="transition-all duration-200 ease-nav-brand">
				<h6 class="mb-0 text-white">Need help?</h6>
				<p class="mt-0 mb-4 text-xs font-semibold leading-tight">Please check our docs</p>
				<a
					href="https://sheba-queue.vercel.app/quick-start/sheba-admin-dashboard/"
					target="_blank"
					class="inline-block w-full px-8 py-2 mb-0 text-xs font-bold text-center text-black uppercase transition-all ease-in bg-white border-0 border-white rounded-lg shadow-soft-md bg-150 leading-pro hover:shadow-soft-2xl hover:scale-102"
				>
					Documentation
				</a>
			</div>
		</div>
	</div>
</aside>
