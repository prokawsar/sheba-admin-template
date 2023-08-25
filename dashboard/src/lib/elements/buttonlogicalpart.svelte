<script>
	import collapse from 'svelte-collapse';

	export let question = '',
		answer = '';

	let open = false;

	import Fa from 'svelte-fa';
	import { faPlus, faMinus } from '@fortawesome/free-solid-svg-icons';
</script>

<div class="flex">
	<button
		class="transition delay-700 flex flex-row gap-1"
		title="Click here to expand"
		on:click={() => (open = !open)}
	>
		<span class="bg-slate-200 hover:bg-blue-100 text-gray-600 hover:text-blue-700 p-1 rounded">
			<Fa icon={!open ? faPlus : faMinus} size="sm" />
		</span>
		<h2 class="font-medium text-slate-700 text-left">
			{question}
		</h2>
	</button>
</div>

<div use:collapse={{ open }}>
	<p class="w-10/12 ml-5 text-sm p-1 text-gray-500 font-medium">
		{answer}
	</p>
</div>
