<script>
	import collapse from 'svelte-collapse';
	let open = true;
	import CollapsableDiv from '$lib/elements/collapsableDiv.svelte';
	import Buttonlogicalpart from '$lib/elements/buttonlogicalpart.svelte';
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

			<Buttonlogicalpart
				question="What platforms are compatible?"
				answer="First, a disclaimer – the entire process of writing a blog post often takes more than a couple
    of hours, even if you can type eighty words as per minute and your writing skills are sharp."
			/>

			<br />

			<Buttonlogicalpart
				question="How many people can it support?"
				answer="First, a disclaimer – the entire process of writing a blog post often takes more than a couple
    of hours, even if you can type eighty words as per minute and your writing skills are sharp."
			/>

			<br />

			<Buttonlogicalpart
				question="How long is the warrianty?"
				answer="First, a disclaimer – the entire process of writing a blog post often takes more than a couple
    of hours, even if you can type eighty words as per minute and your writing skills are sharp."
			/>

			<br />

			<Buttonlogicalpart
				question="How fast is the installation?"
				answer="First, a disclaimer – the entire process of writing a blog post often takes more than a couple
    of hours, even if you can type eighty words as per minute and your writing skills are sharp."
			/>
		</div>
	</div>

	<br /><br />

	<!-- collapse section 2 -->

	<div class="flex justify-around flex-col sm:flex-row">
		<div class="pb-10 sm:pb-0">
			<h2 class="text-2xl">User Roles</h2>
			<br />

			<Buttonlogicalpart
				question="How does it work?"
				answer="First, a disclaimer – the entire process of writing a blog post often takes more than a couple
of hours, even if you can type eighty words as per minute and your writing skills are sharp."
			/>

			<br />

			<Buttonlogicalpart
				question="Do I need a designer to use Admin Theme ?"
				answer="First, a disclaimer – the entire process of writing a blog post often takes more than a couple
of hours, even if you can type eighty words as per minute and your writing skills are sharp."
			/>

			<br />

			<Buttonlogicalpart
				question="What do I need to do to start selling?"
				answer="First, a disclaimer – the entire process of writing a blog post often takes more than a couple
of hours, even if you can type eighty words as per minute and your writing skills are sharp."
			/>

			<br />

			<Buttonlogicalpart
				question="How much does Extended license cost?"
				answer="First, a disclaimer – the entire process of writing a blog post often takes more than a couple
of hours, even if you can type eighty words as per minute and your writing skills are sharp."
			/>
		</div>
		<div class="pb-10 sm:pb-0">
			<h2 class="text-2xl">Installation</h2>
			<br />

			<Buttonlogicalpart
				question="What platforms are compatible?"
				answer="First, a disclaimer – the entire process of writing a blog post often takes more than a couple
of hours, even if you can type eighty words as per minute and your writing skills are sharp."
			/>

			<br />

			<Buttonlogicalpart
				question="How many people can it support?"
				answer="First, a disclaimer – the entire process of writing a blog post often takes more than a couple
of hours, even if you can type eighty words as per minute and your writing skills are sharp."
			/>

			<br />

			<Buttonlogicalpart
				question="How long is the warrianty??"
				answer="First, a disclaimer – the entire process of writing a blog post often takes more than a couple
of hours, even if you can type eighty words as per minute and your writing skills are sharp."
			/>

			<br />

			<Buttonlogicalpart
				question="How fast is the installation?"
				answer="First, a disclaimer – the entire process of writing a blog post often takes more than a couple
of hours, even if you can type eighty words as per minute and your writing skills are sharp."
			/>
		</div>
	</div>
</div>
