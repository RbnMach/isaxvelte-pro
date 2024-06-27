<script lang="ts">
	export let classes = '';
	export let color = 'currentColor';
	export let type: 'linear' | 'bold' | 'broken' | 'bulk' | 'outline' | 'twotone' = 'linear';
	export let size = '1em';
	export let axis_y = '-0.13em';
	export let axis_x = '0';
</script>

<span style="width: {size}; height: {size}; bottom: {axis_y}; left: {axis_x};" class={classes}>
	{#if type == 'linear'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11.2999 14C13.1777 14 14.6999 12.4777 14.6999 10.6C14.6999 8.72218 13.1777 7.19995 11.2999 7.19995C9.42213 7.19995 7.8999 8.72218 7.8999 10.6C7.8999 12.4777 9.42213 14 11.2999 14Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path d="M15.1001 14.8L12.1001 17.8" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16.5 7.3125V7.3125" stroke="{color}" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM7.94 10.56C7.94 8.7 9.45001 7.18 11.32 7.18C13.19 7.18 14.7 8.69 14.7 10.56C14.7 12.43 13.19 13.94 11.32 13.94C9.45001 13.94 7.94 12.43 7.94 10.56ZM15.59 15.34L12.59 18.34C12.44 18.49 12.25 18.56 12.06 18.56C11.87 18.56 11.68 18.49 11.53 18.34C11.24 18.05 11.24 17.57 11.53 17.28L14.53 14.28C14.82 13.99 15.3 13.99 15.59 14.28C15.88 14.57 15.89 15.05 15.59 15.34ZM16.51 8.31C15.96 8.31 15.51 7.86 15.51 7.31C15.51 6.76 15.95 6.31 16.51 6.31H16.52C17.07 6.31 17.52 6.76 17.52 7.31C17.52 7.86 17.06 8.31 16.51 8.31Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11.3097 13.9399C13.1764 13.9399 14.6897 12.4267 14.6897 10.5599C14.6897 8.69321 13.1764 7.17993 11.3097 7.17993C9.44297 7.17993 7.92969 8.69321 7.92969 10.5599C7.92969 12.4267 9.44297 13.9399 11.3097 13.9399Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path d="M15.0605 14.8101L12.0605 17.8101" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.2 2.3 7.97 2.85" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M15.080 18.587c2.489 0 4.507-2.018 4.507-4.507s-2.018-4.507-4.507-4.507c-2.489 0-4.507 2.018-4.507 4.507s2.018 4.507 4.507 4.507z"></path>
<path fill="{color}" d="M22.013 11.080c-0.733 0-1.333-0.6-1.333-1.333s0.587-1.333 1.333-1.333h0.013c0.733 0 1.333 0.6 1.333 1.333-0.013 0.733-0.613 1.333-1.347 1.333z"></path>
<path fill="{color}" d="M16.080 24.747c-0.253 0-0.507-0.093-0.707-0.293-0.387-0.387-0.387-1.027 0-1.413l4-4c0.387-0.387 1.027-0.387 1.413 0s0.387 1.027 0 1.413l-4 4c-0.187 0.2-0.453 0.293-0.707 0.293z"></path>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11.3104 14.6902C9.04042 14.6902 7.19043 12.8402 7.19043 10.5702C7.19043 8.3002 9.04042 6.4502 11.3104 6.4502C13.5804 6.4502 15.4304 8.3002 15.4304 10.5702C15.4304 12.8402 13.5904 14.6902 11.3104 14.6902ZM11.3104 7.9402C9.86042 7.9402 8.69043 9.1202 8.69043 10.5602C8.69043 12.0002 9.87042 13.1802 11.3104 13.1802C12.7504 13.1802 13.9304 12.0002 13.9304 10.5602C13.9304 9.1202 12.7604 7.9402 11.3104 7.9402Z" fill="{color}"/>
<path d="M16.5098 8.31006C15.9598 8.31006 15.5098 7.86006 15.5098 7.31006C15.5098 6.76006 15.9498 6.31006 16.5098 6.31006H16.5198C17.0698 6.31006 17.5198 6.76006 17.5198 7.31006C17.5198 7.86006 17.0598 8.31006 16.5098 8.31006Z" fill="{color}"/>
<path d="M12.06 18.56C11.87 18.56 11.68 18.49 11.53 18.34C11.24 18.05 11.24 17.57 11.53 17.28L14.53 14.28C14.82 13.99 15.3 13.99 15.59 14.28C15.88 14.57 15.88 15.05 15.59 15.34L12.59 18.34C12.45 18.49 12.25 18.56 12.06 18.56Z" fill="{color}"/>
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M11.3097 13.9402C13.1764 13.9402 14.6897 12.4269 14.6897 10.5602C14.6897 8.69345 13.1764 7.18018 11.3097 7.18018C9.44297 7.18018 7.92969 8.69345 7.92969 10.5602C7.92969 12.4269 9.44297 13.9402 11.3097 13.9402Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path opacity="0.4" d="M15.0596 14.8101L12.0596 17.8101" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M17.5 9.3125V9.3125" stroke="{color}" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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
</style>