<script>
	import { faCoins } from '@fortawesome/free-solid-svg-icons';
	import Fa from 'svelte-fa';
</script>

<div class="w-full max-w-full">
	<div
		class="relative flex flex-col min-w-0 break-words bg-white shadow-xl rounded-2xl bg-clip-border"
	>
		<div class="flex-auto p-1 md:p-3">
			<div class="flex flex-row">
				<div class="flex-none w-2/3 max-w-full px-1 sm:px-3">
					<div>
						<p class="mb-0 font-sans text-sm font-semibold leading-normal">Today's Money</p>
						<h5 class="mb-0 font-bold">
							$53,000
							<span class="text-sm leading-normal font-weight-bolder text-lime-500"> +55% </span>
						</h5>
					</div>
				</div>
				<div class="lg:px-3 flex items-center lg:justify-end basis-1/3">
					<div
						class="w-10 h-2/3 sm:w-12 lg:h-full flex justify-center items-center text-center rounded-lg bg-gradient-to-tl from-purple-700 to-pink-500"
					>
						<Fa icon={faCoins} class="text-white" />
					</div>
				</div>
			</div>
		</div>
	</div>
</div>
