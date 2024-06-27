<script lang="ts">
	export let color = 'currentColor';
	export let variant: 'linear' | 'bold' | 'broken' | 'bulk' | 'outline' | 'twotone' = 'linear';
	export let size = '1em';
	export let axis_y = '-0.12em';
	export let axis_x = '0';
	export let flip_x = false;
	export let flip_y = false;
	export let rotate = 0;	
</script>

<span style="width: {size}; height: {size}; bottom: {axis_y}; left: {axis_x}; transform: rotate({rotate}deg);" class:horizontal-reverted={flip_x} class:vertical-reverted={flip_y}>
	{#if variant == 'linear'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5.7 18.4V22L9 20.1C9.9 20.4 10.9 20.5 12 20.5C17.5 20.5 22 16.4 22 11.2C22 6.1 17.5 2 12 2C6.5 2 2 6.1 2 11.3C2 14.2 3.4 16.7 5.7 18.4Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.3 9.19995L7.5 13.7L11.2 12.8L12.7 13.7L16.5 9.19995L13 10.1L11.3 9.19995Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.15001 2 11.26C2 14.16 3.43999 16.74 5.67999 18.44V20.29C5.67999 21.06 6.49998 21.54 7.16998 21.16L9.03003 20.11C9.97003 20.38 10.96 20.52 11.99 20.52C17.51 20.52 21.99 16.37 21.99 11.26C22 6.15001 17.52 2 12 2ZM15.51 10.44L13.01 13.43C12.85 13.62 12.59 13.66 12.38 13.54L11.37 12.95C11.26 12.89 11.13 12.87 11 12.9L8.98999 13.39C8.51999 13.5 8.17999 12.95 8.48999 12.58L11.03 9.56C11.18 9.38 11.44 9.33 11.65 9.44L12.83 10.06C12.94 10.12 13.07 10.13 13.19 10.1L15.01 9.63C15.47 9.51 15.82 10.07 15.51 10.44Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M4.13 5.54999C2.8 7.11999 2 9.11001 2 11.26C2 14.16 3.43999 16.74 5.67999 18.44V22L9.03998 20.11C9.97998 20.38 10.97 20.52 12 20.52C17.52 20.52 22 16.37 22 11.26C22 6.15001 17.52 2 12 2C10.62 2 9.29999 2.26001 8.10999 2.73001" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.28 9.25L7.5 13.75L11.19 12.85L12.74 13.75L16.5 9.25L12.99 10.15L11.28 9.25Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M7.574 24.587v2.467c0 1.027 1.093 1.667 1.987 1.16l2.48-1.4c1.253 0.36 2.573 0.547 3.947 0.547 7.36 0 13.333-5.533 13.333-12.347s-5.973-12.347-13.333-12.347c-7.36 0-13.333 5.533-13.333 12.347 0.013 3.853 1.933 7.307 4.92 9.573z"></path>
<path fill="{color}" d="M14.694 12.747l-3.387 4.027c-0.413 0.493 0.040 1.227 0.667 1.080l2.68-0.653c0.173-0.040 0.347-0.013 0.493 0.067l1.347 0.787c0.28 0.16 0.64 0.107 0.84-0.147l3.333-3.987c0.413-0.493-0.053-1.24-0.68-1.067l-2.427 0.627c-0.16 0.040-0.333 0.027-0.48-0.053l-1.573-0.827c-0.267-0.16-0.613-0.093-0.813 0.147z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5.67999 22.75C5.54999 22.75 5.41999 22.72 5.29999 22.65C5.06999 22.52 4.92999 22.27 4.92999 22V18.8C2.57999 16.89 1.25 14.17 1.25 11.26C1.25 5.74001 6.07 1.25 12 1.25C17.93 1.25 22.75 5.74001 22.75 11.26C22.75 16.78 17.93 21.27 12 21.27C11.03 21.27 10.07 21.15 9.14001 20.91L6.04999 22.65C5.93999 22.72 5.80999 22.75 5.67999 22.75ZM12 2.75C6.9 2.75 2.75 6.57001 2.75 11.26C2.75 13.82 3.98001 16.22 6.14001 17.84C6.33001 17.98 6.44 18.2 6.44 18.44V20.72L8.67999 19.46C8.84999 19.36 9.06 19.34 9.25 19.39C10.14 19.64 11.07 19.77 12 19.77C17.1 19.77 21.25 15.95 21.25 11.26C21.25 6.57001 17.1 2.75 12 2.75Z" fill="{color}"/>
<path d="M7.50019 14.5002C7.25019 14.5002 7.00017 14.3702 6.86017 14.1502C6.69017 13.8702 6.71017 13.5202 6.92017 13.2702L10.7002 8.77019C10.9302 8.50019 11.3102 8.42019 11.6202 8.59019L13.0702 9.36018L16.3002 8.5302C16.6202 8.4502 16.9502 8.58018 17.1202 8.86018C17.2902 9.14018 17.2702 9.49019 17.0602 9.74019L13.3002 14.2402C13.0702 14.5202 12.6602 14.5902 12.3502 14.4102L11.0602 13.6602L7.66016 14.4902C7.62016 14.4902 7.56019 14.5002 7.50019 14.5002ZM11.1902 12.1002C11.3202 12.1002 11.4502 12.1302 11.5702 12.2002L12.5702 12.7802L14.4302 10.5502L13.1702 10.8702C12.9902 10.9202 12.8002 10.8902 12.6302 10.8102L11.4602 10.1902L9.54017 12.4702L11.0002 12.1102C11.0702 12.1102 11.1302 12.1002 11.1902 12.1002Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5.67999 18.44V22L9.03998 20.11C9.97998 20.38 10.97 20.52 12 20.52C17.52 20.52 22 16.37 22 11.26C22 6.15001 17.52 2 12 2C6.48 2 2 6.15001 2 11.26C2 14.15 3.43999 16.74 5.67999 18.44Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M11.28 9.25L7.5 13.75L11.19 12.85L12.74 13.75L16.5 9.25L12.99 10.15L11.28 9.25Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
</span>

<style>
	span {
		display: inline-block;
		stroke-width: 0;
		stroke: currentColor;
		fill: currentColor;
		position: relative;
	}	
	.horizontal-reverted {
		transform: scale(-1, 1);
	}
	.vertical-reverted {
		transform: scale(1, -1);
	}
</style>