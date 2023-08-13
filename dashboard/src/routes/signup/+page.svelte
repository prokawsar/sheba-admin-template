<script>
	import Apple from '$lib/icons/apple.svelte';
	import Facebook from '$lib/icons/facebook.svelte';
	import Google from '$lib/icons/google.svelte';
</script>

<div class="container pt-20">
	<div class="flex flex-wrap">
		<div
			class="w-full max-w-full px-3 mx-auto mt-0 md:flex-0 shrink-0 md:w-7/12 lg:w-5/12 xl:w-4/12"
		>
			<div
				class="outline outline-1 shadow-md outline-teal-500 relative z-0 flex flex-col min-w-0 break-words bg-white border-0 shadow-soft-xl rounded-2xl bg-clip-border"
			>
				<div class="p-6 mb-0 text-center bg-white border-b-0 rounded-t-2xl">
					<h5>Register with</h5>
				</div>
				<div class="flex flex-wrap px-3 sm:px-6 xl:px-12">
					<div class="w-3/12 max-w-full px-1 ml-auto flex-0">
						<a
							class="inline-block w-full px-6 py-3 mb-4 font-bold text-center text-gray-200 uppercase align-middle transition-all bg-transparent border border-gray-200 border-solid rounded-lg shadow-none cursor-pointer hover:scale-102 leading-pro text-xs ease-soft-in tracking-tight-soft bg-150 bg-x-25 hover:bg-transparent hover:opacity-75"
							href="#"
						>
							<Facebook />
						</a>
					</div>
					<div class="w-3/12 max-w-full px-1 flex-0">
						<a
							class="inline-block w-full px-6 py-3 mb-4 font-bold text-center text-gray-200 uppercase align-middle transition-all bg-transparent border border-gray-200 border-solid rounded-lg shadow-none cursor-pointer hover:scale-102 leading-pro text-xs ease-soft-in tracking-tight-soft bg-150 bg-x-25 hover:bg-transparent hover:opacity-75"
							href="#"
						>
							<Apple />
						</a>
					</div>
					<div class="w-3/12 max-w-full px-1 mr-auto flex-0">
						<a
							class="inline-block w-full px-6 py-3 mb-4 font-bold text-center text-gray-200 uppercase align-middle transition-all bg-transparent border border-gray-200 border-solid rounded-lg shadow-none cursor-pointer hover:scale-102 leading-pro text-xs ease-soft-in tracking-tight-soft bg-150 bg-x-25 hover:bg-transparent hover:opacity-75"
							href="#"
						>
							<Google />
						</a>
					</div>
					<div class="relative w-full max-w-full px-3 mt-2 text-center shrink-0">
						<p
							class="z-20 inline px-4 mb-2 font-semibold leading-normal bg-white text-sm text-slate-400"
						>
							or
						</p>
					</div>
				</div>
				<div class="flex-auto p-6">
					<form>
						<div class="mb-4">
							<input
								type="text"
								class="text-sm focus:shadow-soft-primary-outline leading-5.6 ease-soft block w-full appearance-none rounded-lg border-2 border-solid border-gray-300 bg-white bg-clip-padding py-2 px-3 font-normal text-gray-700 transition-all focus:border-teal-300 focus:bg-white focus:text-gray-700 focus:outline-none focus:transition-shadow"
								placeholder="Name"
								aria-label="Name"
								aria-describedby="email-addon"
							/>
						</div>
						<div class="mb-4">
							<input
								type="email"
								class="text-sm focus:shadow-soft-primary-outline leading-5.6 ease-soft block w-full appearance-none rounded-lg border-2 border-solid border-gray-300 bg-white bg-clip-padding py-2 px-3 font-normal text-gray-700 transition-all focus:border-teal-300 focus:bg-white focus:text-gray-700 focus:outline-none focus:transition-shadow"
								placeholder="Email"
								aria-label="Email"
								aria-describedby="email-addon"
							/>
						</div>
						<div class="mb-4">
							<input
								type="password"
								class="text-sm focus:shadow-soft-primary-outline leading-5.6 ease-soft block w-full appearance-none rounded-lg border-2 border-solid border-gray-300 bg-white bg-clip-padding py-2 px-3 font-normal text-gray-700 transition-all focus:border-teal-300 focus:bg-white focus:text-gray-700 focus:outline-none focus:transition-shadow"
								placeholder="Password"
								aria-label="Password"
								aria-describedby="password-addon"
							/>
						</div>
						<div class="min-h-6 pl-6 mb-1 block">
							<input
								id="terms"
								class="w-4 h-4 ease-soft -ml-6 rounded-sm checked:bg-gradient-to-tl checked:from-gray-900 checked:to-slate-800 after:text-xxs after:font-awesome after:duration-250 after:ease-soft-in-out duration-250 relative float-left mt-1 cursor-pointer appearance-none border border-solid border-slate-200 bg-white bg-contain bg-center bg-no-repeat align-top transition-all after:absolute after:rounded-md after:flex after:h-full after:w-full after:items-center after:justify-center after:text-white after:opacity-0 after:transition-all after:content-[''] checked:border-0 checked:border-transparent checked:bg-transparent checked:after:opacity-100"
								type="checkbox"
								value=""
							/>
							<label
								class="mb-2 ml-1 font-normal cursor-pointer select-none text-sm text-slate-700"
								for="terms"
							>
								I agree the
								<a href="" class="font-bold text-slate-700"> Terms and Conditions </a>
							</label>
						</div>
						<div class="text-center">
							<button
								type="button"
								class="inline-block w-full px-6 py-3 mt-6 mb-2 font-bold text-center text-white uppercase align-middle transition-all bg-transparent border-0 rounded-lg cursor-pointer active:opacity-85 hover:scale-102 hover:shadow-soft-xs leading-pro text-xs ease-soft-in tracking-tight-soft shadow-soft-md bg-150 bg-x-25 bg-gradient-to-tl from-gray-900 to-slate-800 hover:border-slate-700 hover:bg-slate-700 hover:text-white"
							>
								Sign up
							</button>
						</div>
						<p class="mt-4 mb-0 leading-normal text-sm">
							Already have an account?
							<a href="/signin" class="font-bold text-slate-700"> Sign in </a>
						</p>
					</form>
				</div>
			</div>
		</div>
	</div>
</div>
