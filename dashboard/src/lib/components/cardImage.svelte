<script>
	import { faArrowRight } from '@fortawesome/free-solid-svg-icons';
	import Fa from 'svelte-fa';
</script>

<div class="w-full mb-6 lg:mb-0 lg:w-7/12">
	<div
		class="relative flex flex-col min-w-0 break-words bg-white shadow-xl rounded-2xl bg-clip-border"
	>
		<div class="flex-auto p-4">
			<div class="flex flex-wrap -mx-3">
				<div class="max-w-full px-3 lg:w-1/2 lg:flex-none">
					<div class="flex flex-col h-full">
						<p class="pt-2 mb-1 font-bold">Built by developers</p>
						<h5 class="font-bold">Sheba Admin Dashboard</h5>
						<p class="mb-12">
							From colors, cards, typography to complex elements, you will find the full
							documentation.
						</p>
						<a
							class="mt-auto mb-0 flex items-center gap-1 text-sm font-semibold leading-normal group text-slate-500"
							href="javascript:;"
						>
							Read More
							<!-- <i
								class="fas fa-arrow-right ease-bounce text-sm group-hover:translate-x-1.25 ml-1 leading-normal transition-all duration-200"
								aria-hidden="true"
							/> -->

							<Fa icon={faArrowRight} />
						</a>
					</div>
				</div>
				<div class="max-w-full px-3 mt-12 ml-auto text-center lg:mt-0 lg:w-5/12 lg:flex-none">
					<div class="h-full bg-gradient-to-tl from-purple-700 to-pink-500 rounded-xl">
						<div class="relative flex items-center justify-center h-full">
							<img
								class="relative z-20 w-full pt-6"
								src="images/illustrations/rocket-white.png"
								alt="rocket"
							/>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</div>
<div class="w-full max-w-full lg:w-5/12">
	<div
		class="border-black/12.5 shadow-xl relative flex h-full min-w-0 flex-col break-words rounded-2xl border-0 border-solid bg-white bg-clip-border p-4"
	>
		<div class="relative h-full overflow-hidden bg-cover rounded-xl">
			<span
				class="absolute top-0 left-0 w-full h-full bg-center bg-cover bg-gradient-to-tl from-gray-900 to-slate-800 opacity-80"
			/>
			<div class="relative flex flex-col flex-auto h-full p-4">
				<h5 class="pt-2 mb-6 font-bold text-white">Work with the rockets</h5>
				<p class="text-white">
					Wealth creation is an evolutionarily recent positive-sum game. It is all about who take
					the opportunity first.
				</p>
				<a
					class="mt-auto mb-0 text-sm flex items-center gap-1 font-semibold leading-normal text-white group"
					href="javascript:;"
				>
					Read More
					<!-- <i
						class="fas fa-arrow-right ease-bounce text-sm group-hover:translate-x-1.25 ml-1 leading-normal transition-all duration-200"
						aria-hidden="true"
					/> -->
					<Fa icon={faArrowRight} />
				</a>
			</div>
		</div>
	</div>
</div>
