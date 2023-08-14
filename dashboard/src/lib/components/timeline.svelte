<script>
	import {
		faArrowUp,
		faBell,
		faCartShopping,
		faCoins,
		faCreditCard,
		faKey,
		faRoad
	} from '@fortawesome/free-solid-svg-icons';
	import Fa from 'svelte-fa';
</script>

<div class="w-full max-w-full md:w-1/2 lg:w-1/3">
	<div
		class="border-black/12.5 shadow-xl relative flex h-full min-w-0 flex-col break-words rounded-2xl border-0 border-solid bg-white bg-clip-border"
	>
		<div class="border-black/12.5 mb-0 rounded-t-2xl border-b-0 border-solid bg-white p-6 pb-0">
			<h6 class="font-bold">Orders overview</h6>
			<p class="text-sm leading-normal flex gap-2 items-center">
				<!-- <i class="fa fa-arrow-up text-lime-500" aria-hidden="true" /> -->
				<Fa icon={faArrowUp} class="text-lime-500" />
				<span class="font-semibold">24%</span>
				this month
			</p>
		</div>
		<div class="flex-auto p-4">
			<div
				class="before:border-r-solid relative before:absolute before:top-0 before:left-4 before:h-full before:border-r-2 before:border-r-slate-100 before:content-[''] before:lg:-ml-px"
			>
				<div class="relative mb-4 mt-0 after:clear-both after:table after:content-['']">
					<span
						class="w-6.5 h-6.5 text-base absolute left-4 z-10 inline-flex -translate-x-1/2 items-center justify-center rounded-full bg-white text-center font-semibold"
					>
						<!-- <i
							class="relative z-10 leading-none text-transparent ni ni-bell-55 leading-pro bg-gradient-to-tl from-green-600 to-lime-400 bg-clip-text fill-transparent"
						/> -->
						<Fa icon={faBell} class="relative z-10 text-green-600 " />
					</span>
					<div class="ml-10 pt-1.4 lg:max-w-120 relative -top-1.5 w-auto">
						<h6 class="mb-0 text-sm font-semibold leading-normal text-slate-700">
							$2400, Design changes
						</h6>
						<p class="mt-1 mb-0 text-xs font-semibold leading-tight text-slate-400">
							22 DEC 7:20 PM
						</p>
					</div>
				</div>
				<div class="relative mb-4 after:clear-both after:table after:content-['']">
					<span
						class="w-6.5 h-6.5 text-base absolute left-4 z-10 inline-flex -translate-x-1/2 items-center justify-center rounded-full bg-white text-center font-semibold"
					>
						<!-- <i
							class="relative z-10 leading-none text-transparent ni ni-html5 leading-pro bg-gradient-to-tl from-red-600 to-rose-400 bg-clip-text fill-transparent"
						/> -->
						<Fa icon={faRoad} class="relative z-10 text-red-600 " />
					</span>
					<div class="ml-10 pt-1.4 lg:max-w-120 relative -top-1.5 w-auto">
						<h6 class="mb-0 text-sm font-semibold leading-normal text-slate-700">
							New order #1832412
						</h6>
						<p class="mt-1 mb-0 text-xs font-semibold leading-tight text-slate-400">21 DEC 11 PM</p>
					</div>
				</div>
				<div class="relative mb-4 after:clear-both after:table after:content-['']">
					<span
						class="w-6.5 h-6.5 text-base absolute left-4 z-10 inline-flex -translate-x-1/2 items-center justify-center rounded-full bg-white text-center font-semibold"
					>
						<!-- <i
							class="relative z-10 leading-none text-transparent ni ni-cart leading-pro bg-gradient-to-tl from-blue-600 to-cyan-400 bg-clip-text fill-transparent"
						/> -->
						<Fa icon={faCartShopping} class="relative z-10 text-blue-600 " />
					</span>
					<div class="ml-10 pt-1.4 lg:max-w-120 relative -top-1.5 w-auto">
						<h6 class="mb-0 text-sm font-semibold leading-normal text-slate-700">
							Server payments for April
						</h6>
						<p class="mt-1 mb-0 text-xs font-semibold leading-tight text-slate-400">
							21 DEC 9:34 PM
						</p>
					</div>
				</div>
				<div class="relative mb-4 after:clear-both after:table after:content-['']">
					<span
						class="w-6.5 h-6.5 text-base absolute left-4 z-10 inline-flex -translate-x-1/2 items-center justify-center rounded-full bg-white text-center font-semibold"
					>
						<!-- <i
							class="relative z-10 leading-none text-transparent ni ni-credit-card leading-pro bg-gradient-to-tl from-red-500 to-yellow-400 bg-clip-text fill-transparent"
						/> -->
						<Fa icon={faCreditCard} class="relative z-10 text-red-500 " />
					</span>
					<div class="ml-10 pt-1.4 lg:max-w-120 relative -top-1.5 w-auto">
						<h6 class="mb-0 text-sm font-semibold leading-normal text-slate-700">
							New card added for order #4395133
						</h6>
						<p class="mt-1 mb-0 text-xs font-semibold leading-tight text-slate-400">
							20 DEC 2:20 AM
						</p>
					</div>
				</div>
				<div class="relative mb-4 after:clear-both after:table after:content-['']">
					<span
						class="w-6.5 h-6.5 text-base absolute left-4 z-10 inline-flex -translate-x-1/2 items-center justify-center rounded-full bg-white text-center font-semibold"
					>
						<i
							class="relative z-10 leading-none text-transparent ni ni-key-25 leading-pro bg-gradient-to-tl from-purple-700 to-pink-500 bg-clip-text fill-transparent"
						/>
						<Fa icon={faKey} class="relative z-10 text-purple-500 " />
					</span>
					<div class="ml-10 pt-1.4 lg:max-w-120 relative -top-1.5 w-auto">
						<h6 class="mb-0 text-sm font-semibold leading-normal text-slate-700">
							Unlock packages for development
						</h6>
						<p class="mt-1 mb-0 text-xs font-semibold leading-tight text-slate-400">
							18 DEC 4:54 AM
						</p>
					</div>
				</div>
				<div class="relative mb-0 after:clear-both after:table after:content-['']">
					<span
						class="w-6.5 h-6.5 text-base absolute left-4 z-10 inline-flex -translate-x-1/2 items-center justify-center rounded-full bg-white text-center font-semibold"
					>
						<i
							class="relative z-10 leading-none text-transparent ni ni-money-coins leading-pro bg-gradient-to-tl from-gray-900 to-slate-800 bg-clip-text fill-transparent"
						/>
						<Fa icon={faCoins} class="relative z-10 text-gray-600 " />
					</span>
					<div class="ml-10 pt-1.4 lg:max-w-120 relative -top-1.5 w-auto">
						<h6 class="mb-0 text-sm font-semibold leading-normal text-slate-700">
							New order #9583120
						</h6>
						<p class="mt-1 mb-0 text-xs font-semibold leading-tight text-slate-400">17 DEC</p>
					</div>
				</div>
			</div>
		</div>
	</div>
</div>
