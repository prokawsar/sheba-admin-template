<script>
	import collapse from 'svelte-collapse';
	import Buttonlogicalpart from './buttonlogicalpart.svelte';
	let open = true;
</script>

<!-- Buying product section  -->

<div class="pb-10 sm:pb-0">
	<h2 class="text-2xl">Buying Product</h2>
	<br />

	<Buttonlogicalpart
		question="How it does it work?"
		answer="First, a disclaimer – the entire process of writing a blog post often takes more than a couple
    of hours, even if you can type eighty words as per minute and your writing skills are sharp."
	/>
	<br />
	<Buttonlogicalpart
		question="Do I need a designer to use Admin Theme ?"
		answer="First, a disclaimer – the entire process of writing a blog post often takes more than a couple of hours, even if you can type eighty words as per minute and your writing skills are sharp."
	/>
	<br />
	<Buttonlogicalpart
		question="What do I need to do to start selling?"
		answer="First, a disclaimer – the entire process of writing a blog post often takes more than a couple of hours, even if you can type eighty words as per minute and your writing skills are sharp."
	/>
	<br />
	<Buttonlogicalpart
		question="How much does Extended license cost?"
		answer="First, a disclaimer – the entire process of writing a blog post often takes more than a couple of hours, even if you can type eighty words as per minute and your writing skills are sharp."
	/>
	<br />
</div>
