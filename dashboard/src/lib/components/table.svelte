<script>
	import { faCheck, faEllipsis } from '@fortawesome/free-solid-svg-icons';
	import Fa from 'svelte-fa';
</script>

<!-- <div class="w-full max-w-full mt-0 md:w-1/2 md:flex-none lg:w-2/3 lg:flex-none"> -->
<div
	class="border-black/10 shadow-xl relative flex min-w-0 flex-col break-words rounded-2xl border-0 border-solid bg-white bg-clip-border"
>
	<div class="border-black/12.5 mb-0 rounded-t-2xl border-b-0 border-solid bg-white p-6 pb-0">
		<div class="flex flex-wrap mt-0 -mx-3">
			<div class="flex-none w-7/12 max-w-full px-3 mt-0 lg:w-1/2 lg:flex-none">
				<h6 class="font-bold">Projects</h6>
				<p class="mb-0 text-sm leading-normal flex items-center">
					<!-- <i class="fa fa-check text-cyan-500" aria-hidden="true" /> -->
					<Fa icon={faCheck} class="text-cyan-500" />
					<span class="ml-1 font-semibold">30 done </span>
					&nbsp; this month
				</p>
			</div>
			<div class="flex-none w-5/12 max-w-full px-3 my-auto text-right lg:w-1/2">
				<div class="relative flex justify-end lg:float-right">
					<a class="cursor-pointer" href="#" aria-expanded="false">
						<Fa icon={faEllipsis} />
					</a>
					<p class="hidden transform-dropdown-show" />

					<ul
						class="z-100 text-sm transform-dropdown shadow-3xl duration-250 before:duration-350 before:font-awesome before:ease-soft min-w-44 -ml-34 before:text-5.5 pointer-events-none absolute top-0 m-0 mt-2 list-none rounded-lg border-0 border-solid border-transparent bg-white bg-clip-padding px-2 py-4 text-left text-slate-500 opacity-0 transition-all before:absolute before:top-0 before:right-7 before:left-auto before:z-40 before:text-white before:transition-all before:content-['\f0d8']"
					>
						<li class="relative">
							<a
								class="py-1.2 lg:ease-soft clear-both block w-full whitespace-nowrap rounded-lg border-0 bg-transparent px-4 text-left font-normal text-slate-500 lg:transition-colors lg:duration-300"
								href="javascript:;"
							>
								Action
							</a>
						</li>
						<li class="relative">
							<a
								class="py-1.2 lg:ease-soft clear-both block w-full whitespace-nowrap rounded-lg border-0 bg-transparent px-4 text-left font-normal text-slate-500 lg:transition-colors lg:duration-300"
								href="javascript:;"
							>
								Another action
							</a>
						</li>
						<li class="relative">
							<a
								class="py-1.2 lg:ease-soft clear-both block w-full whitespace-nowrap rounded-lg border-0 bg-transparent px-4 text-left font-normal text-slate-500 lg:transition-colors lg:duration-300"
								href="javascript:;"
							>
								Something else here
							</a>
						</li>
					</ul>
				</div>
			</div>
		</div>
	</div>
	<div class="flex-auto p-6 px-0 pb-2">
		<div class="overflow-x-auto ps">
			<table class="items-center w-full mb-0 align-top border-gray-200 text-slate-500">
				<thead class="align-bottom">
					<tr>
						<th
							class="px-6 py-3 font-bold tracking-normal text-left uppercase align-middle bg-transparent border-b letter border-b-solid text-xxs whitespace-nowrap border-b-gray-200 text-slate-400 opacity-70"
						>
							Companies
						</th>
						<th
							class="px-6 py-3 pl-2 font-bold tracking-normal text-left uppercase align-middle bg-transparent border-b letter border-b-solid text-xxs whitespace-nowrap border-b-gray-200 text-slate-400 opacity-70"
						>
							Members
						</th>
						<th
							class="px-6 py-3 font-bold tracking-normal text-center uppercase align-middle bg-transparent border-b letter border-b-solid text-xxs whitespace-nowrap border-b-gray-200 text-slate-400 opacity-70"
						>
							Budget
						</th>
						<th
							class="px-6 py-3 font-bold tracking-normal text-center uppercase align-middle bg-transparent border-b letter border-b-solid text-xxs whitespace-nowrap border-b-gray-200 text-slate-400 opacity-70"
						>
							Completion
						</th>
					</tr>
				</thead>
				<tbody>
					<tr>
						<td class="p-2 align-middle bg-transparent border-b whitespace-nowrap">
							<div class="flex px-2 py-1">
								<div>
									<img
										src="/images/small-logos/logo-xd.svg"
										class="inline-flex items-center justify-center mr-4 text-sm text-white transition-all duration-200 ease-soft-in-out h-9 w-9 rounded-xl"
										alt="xd"
									/>
								</div>
								<div class="flex flex-col justify-center">
									<h6 class="mb-0 text-sm leading-normal">Sheba Admin XD Version</h6>
								</div>
							</div>
						</td>
						<td class="p-2 align-middle bg-transparent border-b whitespace-nowrap">
							<!-- <div class="mt-2 avatar-group">
									<a
										href="javascript:;"
										class="relative z-20 inline-flex items-center justify-center w-8 h-8 text-xs text-white transition-all duration-200 border-2 border-white border-solid rounded-full ease-soft-in-out hover:z-30"
										data-target="tooltip_trigger"
										data-placement="bottom"
									>
										<img
											src="/images/people/young-woman.jpg"
											class="w-full rounded-full"
											alt="team1"
										/>
									</a>
									<a
										href="javascript:;"
										class="relative z-20 inline-flex items-center justify-center w-8 h-8 -ml-4 text-xs text-white transition-all duration-200 border-2 border-white border-solid rounded-full ease-soft-in-out hover:z-30"
										data-target="tooltip_trigger"
										data-placement="bottom"
									>
										<img
											src="/images/people/young-woman.jpg"
											class="w-full rounded-full"
											alt="team2"
										/>
									</a>
									<a
										href="javascript:;"
										class="relative z-20 inline-flex items-center justify-center w-8 h-8 -ml-4 text-xs text-white transition-all duration-200 border-2 border-white border-solid rounded-full ease-soft-in-out hover:z-30"
										data-target="tooltip_trigger"
										data-placement="bottom"
									>
										<img
											src="/images/people/young-woman.jpg"
											class="w-full rounded-full"
											alt="team3"
										/>
									</a>
									<a
										href="javascript:;"
										class="relative z-20 inline-flex items-center justify-center w-8 h-8 -ml-4 text-xs text-white transition-all duration-200 border-2 border-white border-solid rounded-full ease-soft-in-out hover:z-30"
										data-target="tooltip_trigger"
										data-placement="bottom"
									>
										<img
											src="/images/people/young-woman.jpg"
											class="w-full rounded-full"
											alt="team4"
										/>
									</a>
								</div> -->
							<div class="flex -space-x-4">
								<img
									class="cursor-pointer z-10 hover:z-20 w-10 h-10 border-2 border-white rounded-full dark:border-gray-800"
									src="/images/people/young-woman.jpg"
									alt=""
								/>
								<img
									class="cursor-pointer z-10 hover:z-20 w-10 h-10 border-2 border-white rounded-full dark:border-gray-800"
									src="/images/people/young-woman.jpg"
									alt=""
								/>
							</div>
						</td>
						<td
							class="p-2 text-sm leading-normal text-center align-middle bg-transparent border-b whitespace-nowrap"
						>
							<span class="text-xs font-semibold leading-tight"> $14,000 </span>
						</td>
						<td class="p-2 align-middle bg-transparent border-b whitespace-nowrap">
							<div class="w-3/4 mx-auto">
								<div>
									<div>
										<span class="text-xs font-semibold leading-tight"> 60% </span>
									</div>
								</div>
								<div class="text-xs h-0.75 w-30 m-0 flex overflow-visible rounded-lg bg-gray-200">
									<div
										class="duration-600 ease-soft bg-gradient-to-tl from-blue-600 to-cyan-400 -mt-0.38 -ml-px flex h-1.5 w-3/5 flex-col justify-center overflow-hidden whitespace-nowrap rounded bg-fuchsia-500 text-center text-white transition-all"
										role="progressbar"
									/>
								</div>
							</div>
						</td>
					</tr>
					<tr>
						<td class="p-2 align-middle bg-transparent border-b whitespace-nowrap">
							<div class="flex px-2 py-1">
								<div>
									<img
										src="/images/small-logos/logo-atlassian.svg"
										class="inline-flex items-center justify-center mr-4 text-sm text-white transition-all duration-200 ease-soft-in-out h-9 w-9 rounded-xl"
										alt="atlassian"
									/>
								</div>
								<div class="flex flex-col justify-center">
									<h6 class="mb-0 text-sm leading-normal">Add Progress Track</h6>
								</div>
							</div>
						</td>
						<td class="p-2 align-middle bg-transparent border-b whitespace-nowrap">
							<div class="flex -space-x-4">
								<img
									class="cursor-pointer z-10 hover:z-20 w-10 h-10 border-2 border-white rounded-full dark:border-gray-800"
									src="/images/people/young-woman.jpg"
									alt=""
								/>
								<img
									class="cursor-pointer z-10 hover:z-20 w-10 h-10 border-2 border-white rounded-full dark:border-gray-800"
									src="/images/people/young-woman.jpg"
									alt=""
								/>
							</div>
						</td>
						<td
							class="p-2 text-sm leading-normal text-center align-middle bg-transparent border-b whitespace-nowrap"
						>
							<span class="text-xs font-semibold leading-tight"> $3,000 </span>
						</td>
						<td class="p-2 align-middle bg-transparent border-b whitespace-nowrap">
							<div class="w-3/4 mx-auto">
								<div>
									<div>
										<span class="text-xs font-semibold leading-tight"> 10% </span>
									</div>
								</div>
								<div class="text-xs h-0.75 w-30 m-0 flex overflow-visible rounded-lg bg-gray-200">
									<div
										class="duration-600 ease-soft bg-gradient-to-tl from-blue-600 to-cyan-400 -mt-0.38 w-1/10 -ml-px flex h-1.5 flex-col justify-center overflow-hidden whitespace-nowrap rounded bg-fuchsia-500 text-center text-white transition-all"
										role="progressbar"
									/>
								</div>
							</div>
						</td>
					</tr>
					<tr>
						<td class="p-2 align-middle bg-transparent border-b whitespace-nowrap">
							<div class="flex px-2 py-1">
								<div>
									<img
										src="/images/small-logos/logo-slack.svg"
										class="inline-flex items-center justify-center mr-4 text-sm text-white transition-all duration-200 ease-soft-in-out h-9 w-9 rounded-xl"
										alt="team7"
									/>
								</div>
								<div class="flex flex-col justify-center">
									<h6 class="mb-0 text-sm leading-normal">Fix Platform Errors</h6>
								</div>
							</div>
						</td>
						<td class="p-2 align-middle bg-transparent border-b whitespace-nowrap">
							<div class="flex -space-x-4">
								<img
									class="cursor-pointer z-10 hover:z-20 w-10 h-10 border-2 border-white rounded-full dark:border-gray-800"
									src="/images/people/young-woman.jpg"
									alt=""
								/>
								<img
									class="cursor-pointer z-10 hover:z-20 w-10 h-10 border-2 border-white rounded-full dark:border-gray-800"
									src="/images/people/young-woman.jpg"
									alt=""
								/>
								<img
									class="cursor-pointer z-10 hover:z-20 w-10 h-10 border-2 border-white rounded-full dark:border-gray-800"
									src="/images/people/young-woman.jpg"
									alt=""
								/>
							</div>
						</td>
						<td
							class="p-2 text-sm leading-normal text-center align-middle bg-transparent border-b whitespace-nowrap"
						>
							<span class="text-xs font-semibold leading-tight"> Not set </span>
						</td>
						<td class="p-2 align-middle bg-transparent border-b whitespace-nowrap">
							<div class="w-3/4 mx-auto">
								<div>
									<div>
										<span class="text-xs font-semibold leading-tight"> 100% </span>
									</div>
								</div>
								<div class="text-xs h-0.75 w-30 m-0 flex overflow-visible rounded-lg bg-gray-200">
									<div
										class="duration-600 ease-soft bg-gradient-to-tl from-green-600 to-lime-400 -mt-0.38 -ml-px flex h-1.5 w-full flex-col justify-center overflow-hidden whitespace-nowrap rounded bg-fuchsia-500 text-center text-white transition-all"
										role="progressbar"
									/>
								</div>
							</div>
						</td>
					</tr>
					<tr>
						<td class="p-2 align-middle bg-transparent border-b whitespace-nowrap">
							<div class="flex px-2 py-1">
								<div>
									<img
										src="/images/small-logos/logo-spotify.svg"
										class="inline-flex items-center justify-center mr-4 text-sm text-white transition-all duration-200 ease-soft-in-out h-9 w-9 rounded-xl"
										alt="spotify"
									/>
								</div>
								<div class="flex flex-col justify-center">
									<h6 class="mb-0 text-sm leading-normal">Launch our Mobile App</h6>
								</div>
							</div>
						</td>
						<td class="p-2 align-middle bg-transparent border-b whitespace-nowrap">
							<div class="flex -space-x-4">
								<img
									class="cursor-pointer z-10 hover:z-20 w-10 h-10 border-2 border-white rounded-full dark:border-gray-800"
									src="/images/people/young-woman.jpg"
									alt=""
								/>
								<img
									class="cursor-pointer z-10 hover:z-20 w-10 h-10 border-2 border-white rounded-full dark:border-gray-800"
									src="/images/people/young-woman.jpg"
									alt=""
								/>
							</div>
						</td>
						<td
							class="p-2 text-sm leading-normal text-center align-middle bg-transparent border-b whitespace-nowrap"
						>
							<span class="text-xs font-semibold leading-tight"> $20,500 </span>
						</td>
						<td class="p-2 align-middle bg-transparent border-b whitespace-nowrap">
							<div class="w-3/4 mx-auto">
								<div>
									<div>
										<span class="text-xs font-semibold leading-tight"> 100% </span>
									</div>
								</div>
								<div class="text-xs h-0.75 w-30 m-0 flex overflow-visible rounded-lg bg-gray-200">
									<div
										class="duration-600 ease-soft bg-gradient-to-tl from-green-600 to-lime-400 -mt-0.38 -ml-px flex h-1.5 w-full flex-col justify-center overflow-hidden whitespace-nowrap rounded bg-fuchsia-500 text-center text-white transition-all"
										role="progressbar"
									/>
								</div>
							</div>
						</td>
					</tr>
					<tr>
						<td class="p-2 align-middle bg-transparent border-b whitespace-nowrap">
							<div class="flex px-2 py-1">
								<div>
									<img
										src="/images/small-logos/logo-jira.svg"
										class="inline-flex items-center justify-center mr-4 text-sm text-white transition-all duration-200 ease-soft-in-out h-9 w-9 rounded-xl"
										alt="jira"
									/>
								</div>
								<div class="flex flex-col justify-center">
									<h6 class="mb-0 text-sm leading-normal">Add the New Pricing Page</h6>
								</div>
							</div>
						</td>
						<td class="p-2 align-middle bg-transparent border-b whitespace-nowrap">
							<div class="flex -space-x-4">
								<img
									class="cursor-pointer z-10 hover:z-20 w-10 h-10 border-2 border-white rounded-full dark:border-gray-800"
									src="/images/people/young-woman.jpg"
									alt=""
								/>
								<img
									class="cursor-pointer z-10 hover:z-20 w-10 h-10 border-2 border-white rounded-full dark:border-gray-800"
									src="/images/people/young-woman.jpg"
									alt=""
								/>
								<img
									class="cursor-pointer z-10 hover:z-20 w-10 h-10 border-2 border-white rounded-full dark:border-gray-800"
									src="/images/people/young-woman.jpg"
									alt=""
								/>
								<img
									class="cursor-pointer z-10 hover:z-20 w-10 h-10 border-2 border-white rounded-full dark:border-gray-800"
									src="/images/people/young-woman.jpg"
									alt=""
								/>
							</div>
						</td>
						<td
							class="p-2 text-sm leading-normal text-center align-middle bg-transparent border-b whitespace-nowrap"
						>
							<span class="text-xs font-semibold leading-tight"> $500 </span>
						</td>
						<td class="p-2 align-middle bg-transparent border-b whitespace-nowrap">
							<div class="w-3/4 mx-auto">
								<div>
									<div>
										<span class="text-xs font-semibold leading-tight"> 25% </span>
									</div>
								</div>
								<div class="text-xs h-0.75 w-30 m-0 flex overflow-visible rounded-lg bg-gray-200">
									<div
										class="duration-600 ease-soft bg-gradient-to-tl from-blue-600 to-cyan-400 -mt-0.38 -ml-px flex h-1.5 w-1/4 flex-col justify-center overflow-hidden whitespace-nowrap rounded bg-fuchsia-500 text-center text-white transition-all"
										role="progressbar"
									/>
								</div>
							</div>
						</td>
					</tr>
					<tr>
						<td class="p-2 align-middle bg-transparent border-0 whitespace-nowrap">
							<div class="flex px-2 py-1">
								<div>
									<img
										src="/images/small-logos/logo-invision.svg"
										class="inline-flex items-center justify-center mr-4 text-sm text-white transition-all duration-200 ease-soft-in-out h-9 w-9 rounded-xl"
										alt="invision"
									/>
								</div>
								<div class="flex flex-col justify-center">
									<h6 class="mb-0 text-sm leading-normal">Redesign New Online Shop</h6>
								</div>
							</div>
						</td>
						<td class="p-2 align-middle bg-transparent border-0 whitespace-nowrap">
							<div class="flex -space-x-4">
								<img
									class="cursor-pointer z-10 hover:z-20 w-10 h-10 border-2 border-white rounded-full dark:border-gray-800"
									src="/images/people/young-woman.jpg"
									alt=""
								/>
								<img
									class="cursor-pointer z-10 hover:z-20 w-10 h-10 border-2 border-white rounded-full dark:border-gray-800"
									src="/images/people/young-woman.jpg"
									alt=""
								/>
							</div>
						</td>
						<td
							class="p-2 text-sm leading-normal text-center align-middle bg-transparent border-0 whitespace-nowrap"
						>
							<span class="text-xs font-semibold leading-tight"> $2,000 </span>
						</td>
						<td class="p-2 align-middle bg-transparent border-0 whitespace-nowrap">
							<div class="w-3/4 mx-auto">
								<div>
									<div>
										<span class="text-xs font-semibold leading-tight"> 40% </span>
									</div>
								</div>
								<div class="text-xs h-0.75 w-30 m-0 flex overflow-visible rounded-lg bg-gray-200">
									<div
										class="duration-600 ease-soft bg-gradient-to-tl from-blue-600 to-cyan-400 -mt-0.38 -ml-px flex h-1.5 w-2/5 flex-col justify-center overflow-hidden whitespace-nowrap rounded bg-fuchsia-500 text-center text-white transition-all"
										role="progressbar"
									/>
								</div>
							</div>
						</td>
					</tr>
				</tbody>
			</table>
		</div>
	</div>
</div>
<!-- </div> -->