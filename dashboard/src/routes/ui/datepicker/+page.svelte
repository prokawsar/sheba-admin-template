<script>
	import Datepicker from '$lib/elements/datepicker.svelte';
</script>

<div class="container mx-auto">
	<div class="flex">
		<Datepicker
			value=""
			style=""
			class="w-full p-2 mx-4 outline-2 outline-teal-300"
			placeholder="Select Date.."
			disabled={false}
			enable_dates={[]}
			disable_dates={[]}
			range_mode={false}
			options={{}}
			calendar_color="primary"
			color=""
			readonly={false}
		/>
	</div>
</div>
