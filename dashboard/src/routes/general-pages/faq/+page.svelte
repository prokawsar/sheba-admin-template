<script>
	import collapse from 'svelte-collapse';
	let open = true;
	import CollapsableDiv from '$lib/elements/collapsableDiv.svelte';
</script>

<div class="pt-7 pl-7 pr-6 sm:pt-16 sm:pl-20 sm:pr-0 mb-10 sm:mb-10">
	<h2 class="text-3xl font-medium">Frequesntly Asked Questions</h2>
	<br />
	<p class="text-lg w-11/12">
		First, a disclaimer – the entire process of writing a blog post often takes more than a couple
		of hours, even if you can type eighty words as per minute and your writing skills are sharp.
	</p>

	<br /> <br />

	<!-- collapse section 1 -->

	<div class="flex justify-around flex-col sm:flex-row">
		<CollapsableDiv />
		<div class="pb-10 sm:pb-0">
			<h2 class="text-2xl">Installation</h2>
			<br />
			<button title="Click here to expand" on:click={() => (open = !open)}>
				What platforms are compatible?
			</button>
			<div use:collapse={{ open }}>
				<p>
					First, a disclaimer – the entire process of writing a blog post often takes more than a
					couple of hours, even if you can type eighty words as per minute and your writing skills
					are sharp.
				</p>
			</div>

			<br />
			<button title="Click here to expand" on:click={() => (open = !open)}>
				How many people can it support?
			</button>
			<div use:collapse={{ open }}>
				<p>
					First, a disclaimer – the entire process of writing a blog post often takes more than a
					couple of hours, even if you can type eighty words as per minute and your writing skills
					are sharp.
				</p>
			</div>

			<br />
			<button title="Click here to expand" on:click={() => (open = !open)}>
				How long is the warrianty?
			</button>
			<div use:collapse={{ open }}>
				<p>
					First, a disclaimer – the entire process of writing a blog post often takes more than a
					couple of hours, even if you can type eighty words as per minute and your writing skills
					are sharp.
				</p>
			</div>

			<br />
			<button title="Click here to expand" on:click={() => (open = !open)}>
				How fast is the installation?
			</button>
			<div use:collapse={{ open }}>
				<p>
					First, a disclaimer – the entire process of writing a blog post often takes more than a
					couple of hours, even if you can type eighty words as per minute and your writing skills
					are sharp.
				</p>
			</div>
		</div>
	</div>

	<br /><br />

	<!-- collapse section 2 -->

	<div class="flex justify-around flex-col sm:flex-row">
		<div class="pb-10 sm:pb-0">
			<h2 class="text-2xl">User Roles</h2>
			<br />
			<button title="Click here to expand" on:click={() => (open = !open)}>
				How does it work?
			</button>
			<div use:collapse={{ open }}>
				<p>
					First, a disclaimer – the entire process of writing a blog post often takes more than a
					couple of hours, even if you can type eighty words as per minute and your writing skills
					are sharp.
				</p>
			</div>

			<br />
			<button title="Click here to expand" on:click={() => (open = !open)}>
				Do I need a designer to use Admin Theme ?
			</button>
			<div use:collapse={{ open }}>
				<p>
					First, a disclaimer – the entire process of writing a blog post often takes more than a
					couple of hours, even if you can type eighty words as per minute and your writing skills
					are sharp.
				</p>
			</div>

			<br />
			<button title="Click here to expand" on:click={() => (open = !open)}>
				What do I need to do to start selling?
			</button>
			<div use:collapse={{ open }}>
				<p>
					First, a disclaimer – the entire process of writing a blog post often takes more than a
					couple of hours, even if you can type eighty words as per minute and your writing skills
					are sharp.
				</p>
			</div>

			<br />
			<button title="Click here to expand" on:click={() => (open = !open)}>
				How much does Extended license cost?
			</button>
			<div use:collapse={{ open }}>
				<p>
					First, a disclaimer – the entire process of writing a blog post often takes more than a
					couple of hours, even if you can type eighty words as per minute and your writing skills
					are sharp.
				</p>
			</div>
		</div>
		<div class="pb-10 sm:pb-0">
			<h2 class="text-2xl">Installation</h2>
			<br />
			<button title="Click here to expand" on:click={() => (open = !open)}>
				What platforms are compatible?
			</button>
			<div use:collapse={{ open }}>
				<p>
					First, a disclaimer – the entire process of writing a blog post often takes more than a
					couple of hours, even if you can type eighty words as per minute and your writing skills
					are sharp.
				</p>
			</div>

			<br />
			<button title="Click here to expand" on:click={() => (open = !open)}>
				How many people can it support?
			</button>
			<div use:collapse={{ open }}>
				<p>
					First, a disclaimer – the entire process of writing a blog post often takes more than a
					couple of hours, even if you can type eighty words as per minute and your writing skills
					are sharp.
				</p>
			</div>

			<br />
			<button title="Click here to expand" on:click={() => (open = !open)}>
				How long is the warrianty?
			</button>
			<div use:collapse={{ open }}>
				<p>
					First, a disclaimer – the entire process of writing a blog post often takes more than a
					couple of hours, even if you can type eighty words as per minute and your writing skills
					are sharp.
				</p>
			</div>

			<br />
			<button title="Click here to expand" on:click={() => (open = !open)}>
				How fast is the installation?
			</button>
			<div use:collapse={{ open }}>
				<p>
					First, a disclaimer – the entire process of writing a blog post often takes more than a
					couple of hours, even if you can type eighty words as per minute and your writing skills
					are sharp.
				</p>
			</div>
		</div>
	</div>
</div>
