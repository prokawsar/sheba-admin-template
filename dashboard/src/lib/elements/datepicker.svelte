<script lang="ts">
	import { createEventDispatcher, onMount } from 'svelte';
	import flatpickr from 'flatpickr';
	import 'flatpickr/dist/flatpickr.min.css';

	const fire = createEventDispatcher();

	export let value = '';
	export let style = '';
	/**
	 * Colour of the Date picker input
	 */
	export let color = '';
	/**
	 * Disables the component
	 */
	export let disabled = false;
	/**
	 * Make input value read-only
	 */
	export let readonly = false;
	/**
	 * Placeholder text for the input
	 */
	export let placeholder = 'Select Date..';
	/**
	 * Colour of the Calendar
	 */
	export let calendar_color = 'primary';
	/**
	 * Set earliest selectable date as an object or string
	 *
	 * **Example:** `"2021-06-06"` or `"(new Date('2021-01-01'))"`
	 * @type {any}
	 */
	export let min_date = null;
	/**
	 * Set latest selectable date as an object or string
	 *
	 * **Example:** `"2021-06-06"` or `"(new Date('2021-01-01'))"`
	 * @type {any}
	 */
	export let max_date = null;
	/**
	 * Enables a range of dates and disables all others
	 * @type {array}
	 */
	export let enable_dates: any[] = [];
	/**
	 * Disables a range of dates and enables all others
	 * @type {array}
	 */
	export let disable_dates: any[] = [];
	/**
	 * Allows selecting a date range
	 */
	export let range_mode = false;

	/**
	 * Extended set of options as supported by Flatpicker
	 *
	 * See: https://flatpickr.js.org/options/
	 */
	export let options = {};
	/**
	 * CSS classes for the input
	 */
	let klass = '';
	export { klass as class };

	let opts: any;

	let refDatePicker: any;

	onMount(() => {
		if (refDatePicker) {
			flatpickr(refDatePicker, {});
		}
	});
</script>

<!--Native input change event-->
<input
	bind:this={refDatePicker}
	class={klass}
	type="text"
	{style}
	{placeholder}
	{disabled}
	readonly
	bind:value
	on:change
/>
