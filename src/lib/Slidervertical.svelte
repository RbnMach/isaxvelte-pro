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
<path d="M7.5 5H16.5C17.12 5 17.67 5.02 18.16 5.09C20.79 5.38 21.5 6.62 21.5 10V14C21.5 17.38 20.79 18.62 18.16 18.91C17.67 18.98 17.12 19 16.5 19H7.5C6.88 19 6.33 18.98 5.84 18.91C3.21 18.62 2.5 17.38 2.5 14V10C2.5 6.62 3.21 5.38 5.84 5.09C6.33 5.02 6.88 5 7.5 5Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4.5 2H19.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5 22H20" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M18.9405 3.5H5.06055C4.65055 3.5 4.31055 3.16 4.31055 2.75C4.31055 2.34 4.65055 2 5.06055 2H18.9405C19.3505 2 19.6905 2.34 19.6905 2.75C19.6905 3.16 19.3505 3.5 18.9405 3.5Z" fill="{color}"/>
<path d="M18.9405 22H5.06055C4.65055 22 4.31055 21.66 4.31055 21.25C4.31055 20.84 4.65055 20.5 5.06055 20.5H18.9405C19.3505 20.5 19.6905 20.84 19.6905 21.25C19.6905 21.66 19.3505 22 18.9405 22Z" fill="{color}"/>
<path d="M2.75 8V16C2.75 17.66 4.09 19 5.75 19H18.25C19.91 19 21.25 17.66 21.25 16V8C21.25 6.34 19.91 5 18.25 5H5.75C4.09 5 2.75 6.34 2.75 8Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11.55 5H16.5C17.12 5 17.67 5.02 18.16 5.09C20.79 5.38 21.5 6.62 21.5 10V14C21.5 17.38 20.79 18.62 18.16 18.91C17.67 18.98 17.12 19 16.5 19H7.5C6.88 19 6.33 18.98 5.84 18.91C3.21 18.62 2.5 17.38 2.5 14V10C2.5 6.62 3.21 5.38 5.84 5.09C6.33 5.02 6.88 5 7.5 5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4.5 2H19.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5 22H20" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M18.9405 3.5H5.06055C4.65055 3.5 4.31055 3.16 4.31055 2.75C4.31055 2.34 4.65055 2 5.06055 2H18.9405C19.3505 2 19.6905 2.34 19.6905 2.75C19.6905 3.16 19.3505 3.5 18.9405 3.5Z" fill="{color}"/>
<path d="M18.9405 22H5.06055C4.65055 22 4.31055 21.66 4.31055 21.25C4.31055 20.84 4.65055 20.5 5.06055 20.5H18.9405C19.3505 20.5 19.6905 20.84 19.6905 21.25C19.6905 21.66 19.3505 22 18.9405 22Z" fill="{color}"/>
<path opacity="0.4" d="M2.75 7.6001V16.4001C2.75 18.0601 4.09 19.4001 5.75 19.4001H18.25C19.91 19.4001 21.25 18.0601 21.25 16.4001V7.6001C21.25 5.9401 19.91 4.6001 18.25 4.6001H5.75C4.09 4.6001 2.75 5.9401 2.75 7.6001Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.5 19.75H7.5C6.75 19.75 6.2 19.72 5.73 19.65C2.41 19.29 1.75 17.3 1.75 14V10C1.75 6.7 2.41 4.71 5.76 4.34C6.2 4.28 6.75 4.25 7.5 4.25H16.5C17.25 4.25 17.8 4.28 18.27 4.35C21.6 4.72 22.25 6.7 22.25 10V14C22.25 17.3 21.59 19.29 18.24 19.66C17.8 19.72 17.25 19.75 16.5 19.75ZM7.5 5.75C6.82 5.75 6.34 5.78 5.95 5.83C3.92 6.06 3.25 6.69 3.25 10V14C3.25 17.31 3.92 17.94 5.92 18.17C6.34 18.23 6.82 18.25 7.5 18.25H16.5C17.18 18.25 17.66 18.22 18.05 18.17C20.08 17.95 20.75 17.31 20.75 14V10C20.75 6.69 20.08 6.06 18.08 5.83C17.66 5.77 17.18 5.75 16.5 5.75H7.5Z" fill="{color}"/>
<path d="M19.5 2.75H4.5C4.09 2.75 3.75 2.41 3.75 2C3.75 1.59 4.09 1.25 4.5 1.25H19.5C19.91 1.25 20.25 1.59 20.25 2C20.25 2.41 19.91 2.75 19.5 2.75Z" fill="{color}"/>
<path d="M20 22.75H5C4.59 22.75 4.25 22.41 4.25 22C4.25 21.59 4.59 21.25 5 21.25H20C20.41 21.25 20.75 21.59 20.75 22C20.75 22.41 20.41 22.75 20 22.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M7.5 5H16.5C17.12 5 17.67 5.02 18.16 5.09C20.79 5.38 21.5 6.62 21.5 10V14C21.5 17.38 20.79 18.62 18.16 18.91C17.67 18.98 17.12 19 16.5 19H7.5C6.88 19 6.33 18.98 5.84 18.91C3.21 18.62 2.5 17.38 2.5 14V10C2.5 6.62 3.21 5.38 5.84 5.09C6.33 5.02 6.88 5 7.5 5Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M4.5 2H19.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M5 22H20" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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