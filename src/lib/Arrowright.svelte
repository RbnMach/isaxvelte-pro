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
<path d="M14.4301 5.92993L20.5001 11.9999L14.4301 18.0699" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3.5 12H20.33" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.19 2H7.81C4.17 2 2 4.17 2 7.81V16.18C2 19.83 4.17 22 7.81 22H16.18C19.82 22 21.99 19.83 21.99 16.19V7.81C22 4.17 19.83 2 16.19 2ZM18.53 12.53L14.24 16.82C14.09 16.97 13.9 17.04 13.71 17.04C13.52 17.04 13.33 16.97 13.18 16.82C12.89 16.53 12.89 16.05 13.18 15.76L16.19 12.75H6C5.59 12.75 5.25 12.41 5.25 12C5.25 11.59 5.59 11.25 6 11.25H16.19L13.18 8.24C12.89 7.95 12.89 7.47 13.18 7.18C13.47 6.89 13.95 6.89 14.24 7.18L18.53 11.47C18.67 11.61 18.75 11.8 18.75 12C18.75 12.2 18.67 12.39 18.53 12.53Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M14.4297 5.92993L20.4997 11.9999L14.4297 18.0699" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.0098 12H20.3298" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3.5 12H6.97" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M16.19 2H7.81C4.17 2 2 4.17 2 7.81V16.18C2 19.83 4.17 22 7.81 22H16.18C19.82 22 21.99 19.83 21.99 16.19V7.81C22 4.17 19.83 2 16.19 2Z" fill="{color}"/>
<path d="M18.53 11.4699L14.24 7.1799C13.95 6.8899 13.47 6.8899 13.18 7.1799C12.89 7.4699 12.89 7.9499 13.18 8.2399L16.19 11.2499H6C5.59 11.2499 5.25 11.5899 5.25 11.9999C5.25 12.4099 5.59 12.7499 6 12.7499H16.19L13.18 15.7599C12.89 16.0499 12.89 16.5299 13.18 16.8199C13.33 16.9699 13.52 17.0399 13.71 17.0399C13.9 17.0399 14.09 16.9699 14.24 16.8199L18.53 12.5299C18.67 12.3899 18.75 12.1999 18.75 11.9999C18.75 11.7999 18.67 11.6099 18.53 11.4699Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M14.4291 18.8201C14.2391 18.8201 14.0491 18.7501 13.8991 18.6001C13.6091 18.3101 13.6091 17.8301 13.8991 17.5401L19.4391 12.0001L13.8991 6.46012C13.6091 6.17012 13.6091 5.69012 13.8991 5.40012C14.1891 5.11012 14.6691 5.11012 14.9591 5.40012L21.0291 11.4701C21.3191 11.7601 21.3191 12.2401 21.0291 12.5301L14.9591 18.6001C14.8091 18.7501 14.6191 18.8201 14.4291 18.8201Z" fill="{color}"/>
<path d="M20.33 12.75H3.5C3.09 12.75 2.75 12.41 2.75 12C2.75 11.59 3.09 11.25 3.5 11.25H20.33C20.74 11.25 21.08 11.59 21.08 12C21.08 12.41 20.74 12.75 20.33 12.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M14.4297 5.93018L20.4997 12.0002L14.4297 18.0702" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M3.5 12H20.33" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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