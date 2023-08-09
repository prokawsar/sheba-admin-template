<script>
	import Box_3d from '$lib/icons/box-3d.svelte';
	import Credit from '$lib/icons/credit.svelte';
	import Customer from '$lib/icons/customer.svelte';
	import Document from '$lib/icons/document.svelte';
	import Office from '$lib/icons/office.svelte';
	import Settings from '$lib/icons/settings.svelte';
	import Shop from '$lib/icons/shop.svelte';
	import Spaceship from '$lib/icons/spaceship.svelte';
</script>

<aside class="max-w-xs block w-full fixed flex-wrap">
	<div class="h-20">
		<i
			class="absolute top-0 right-0 hidden p-4 opacity-50 cursor-pointer fas fa-times text-slate-400 xl:hidden"
			aria-hidden="true"
		/>
		<a
			class="block px-8 py-6 m-0 text-sm whitespace-nowrap text-slate-700"
			href="javascript:;"
			target="_blank"
		>
			<span class="ml-1 font-semibold transition-all duration-200 ease-nav-brand">
				Sheba Admin Dashboard
			</span>
		</a>
	</div>

	<hr
		class="h-px mt-0 bg-transparent bg-gradient-to-r from-transparent via-black/40 to-transparent"
	/>

	<div class="items-center block w-auto max-h-screen overflow-auto grow basis-full">
		<ul class="flex flex-col pl-0 mb-0">
			<li class="mt-1 w-full">
				<a
					class="py-2 shadow-xl text-sm ease-nav-brand my-0 mx-4 flex items-center whitespace-nowrap rounded-lg bg-white px-4 font-semibold text-slate-700 transition-colors"
					href="./pages/dashboard.html"
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

			<li class="mt-1 w-full">
				<a
					class="py-2 text-sm ease-nav-brand my-0 mx-4 flex items-center whitespace-nowrap px-4 transition-colors"
					href="./pages/tables.html"
				>
					<div
						class="shadow-xl mr-2 flex h-8 w-8 items-center justify-center rounded-lg bg-white bg-center stroke-0 text-center xl:p-2"
					>
						<Office />
					</div>
					<span class="ml-1 duration-300 opacity-100 pointer-events-none ease-soft"> Tables </span>
				</a>
			</li>

			<li class="mt-1 w-full">
				<a
					class="py-2 text-sm ease-nav-brand my-0 mx-4 flex items-center whitespace-nowrap px-4 transition-colors"
					href="./pages/billing.html"
				>
					<div
						class="shadow-xl mr-2 flex h-8 w-8 items-center justify-center rounded-lg bg-white bg-center fill-current stroke-0 text-center xl:p-2"
					>
						<Credit />
					</div>
					<span class="ml-1 duration-300 opacity-100 pointer-events-none ease-soft"> Billing </span>
				</a>
			</li>

			<li class="mt-1 w-full">
				<a
					class="py-2 text-sm ease-nav-brand my-0 mx-4 flex items-center whitespace-nowrap px-4 transition-colors"
					href="./pages/virtual-reality.html"
				>
					<div
						class="shadow-xl mr-2 flex h-8 w-8 items-center justify-center rounded-lg bg-white bg-center stroke-0 text-center xl:p-2"
					>
						<Box_3d />
					</div>
					<span class="ml-1 duration-300 opacity-100 pointer-events-none ease-soft">
						Virtual Reality
					</span>
				</a>
			</li>

			<li class="mt-1 w-full">
				<a
					class="py-2 text-sm ease-nav-brand my-0 mx-4 flex items-center whitespace-nowrap px-4 transition-colors"
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

			<li class="mt-1 w-full">
				<a
					class="py-2 text-sm ease-nav-brand my-0 mx-4 flex items-center whitespace-nowrap px-4 transition-colors"
					href="./pages/profile.html"
				>
					<div
						class="shadow-xl mr-2 flex h-8 w-8 items-center justify-center rounded-lg bg-white bg-center stroke-0 text-center xl:p-2"
					>
						<Customer />
					</div>
					<span class="ml-1 duration-300 opacity-100 pointer-events-none ease-soft"> Profile </span>
				</a>
			</li>

			<li class="mt-1 w-full">
				<a
					class="py-2 text-sm ease-nav-brand my-0 mx-4 flex items-center whitespace-nowrap px-4 transition-colors"
					href="./pages/sign-in.html"
				>
					<div
						class="shadow-xl mr-2 flex h-8 w-8 items-center justify-center rounded-lg bg-white bg-center stroke-0 text-center xl:p-2"
					>
						<Document />
					</div>
					<span class="ml-1 duration-300 opacity-100 pointer-events-none ease-soft"> Sign In </span>
				</a>
			</li>

			<li class="mt-1 w-full">
				<a
					class="py-2 text-sm ease-nav-brand my-0 mx-4 flex items-center whitespace-nowrap px-4 transition-colors"
					href="./pages/sign-up.html"
				>
					<div
						class="shadow-xl mr-2 flex h-8 w-8 items-center justify-center rounded-lg bg-white bg-center stroke-0 text-center xl:p-2"
					>
						<Spaceship />
					</div>
					<span class="ml-1 duration-300 opacity-100 pointer-events-none ease-soft"> Sign Up </span>
				</a>
			</li>
		</ul>
	</div>
</aside>
