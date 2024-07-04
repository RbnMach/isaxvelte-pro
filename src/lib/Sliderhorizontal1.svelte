<script lang="ts">
	export let color = 'currentColor';
	export let variant: 'linear' | 'bold' | 'broken' | 'bulk' | 'outline' | 'twotone' = 'linear';
	export let size = '1.1em';
	export let axis_y = '-0.13em';
	export let axis_x = '0';
	export let flip_x = false;
	export let flip_y = false;
	export let rotate = 0;	
</script>

<span style="width: {size}; height: {size}; bottom: {axis_y}; left: {axis_x}; transform: rotate({rotate}deg);" class:horizontal-reverted={flip_x} class:vertical-reverted={flip_y}>
	{#if variant == 'linear'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5 16.5V7.5C5 6.88 5.02 6.33 5.09 5.84C5.38 3.21 6.62 2.5 10 2.5H14C17.38 2.5 18.62 3.21 18.91 5.84C18.98 6.33 19 6.88 19 7.5V16.5C19 17.12 18.98 17.67 18.91 18.16C18.62 20.79 17.38 21.5 14 21.5H10C6.62 21.5 5.38 20.79 5.09 18.16C5.02 17.67 5 17.12 5 16.5Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 19.5V4.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M22 19V4" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M3.5 5.05859V18.9386C3.5 19.3486 3.16 19.6886 2.75 19.6886C2.34 19.6886 2 19.3486 2 18.9386V5.05859C2 4.64859 2.34 4.30859 2.75 4.30859C3.16 4.30859 3.5 4.64859 3.5 5.05859Z" fill="{color}"/>
<path d="M22 5.05859V18.9386C22 19.3486 21.66 19.6886 21.25 19.6886C20.84 19.6886 20.5 19.3486 20.5 18.9386V5.05859C20.5 4.64859 20.84 4.30859 21.25 4.30859C21.66 4.30859 22 4.64859 22 5.05859Z" fill="{color}"/>
<path d="M8 21.25H16C17.66 21.25 19 19.91 19 18.25V5.75C19 4.09 17.66 2.75 16 2.75H8C6.34 2.75 5 4.09 5 5.75V18.25C5 19.91 6.34 21.25 8 21.25Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2 19.5V4.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M22 19V4" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5 12.45V7.5C5 6.88 5.02 6.33 5.09 5.84C5.38 3.21 6.62 2.5 10 2.5H14C17.38 2.5 18.62 3.21 18.91 5.84C18.98 6.33 19 6.88 19 7.5V16.5C19 17.12 18.98 17.67 18.91 18.16C18.62 20.79 17.38 21.5 14 21.5H10C6.62 21.5 5.38 20.79 5.09 18.16C5.02 17.67 5 17.12 5 16.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M3.5 5.06006V18.9401C3.5 19.3501 3.16 19.6901 2.75 19.6901C2.34 19.6901 2 19.3501 2 18.9401V5.06006C2 4.65006 2.34 4.31006 2.75 4.31006C3.16 4.31006 3.5 4.65006 3.5 5.06006Z" fill="{color}"/>
<path d="M22 5.06006V18.9401C22 19.3501 21.66 19.6901 21.25 19.6901C20.84 19.6901 20.5 19.3501 20.5 18.9401V5.06006C20.5 4.65006 20.84 4.31006 21.25 4.31006C21.66 4.31006 22 4.65006 22 5.06006Z" fill="{color}"/>
<path opacity="0.4" d="M7.59961 21.25H16.3996C18.0596 21.25 19.3996 19.91 19.3996 18.25V5.75C19.3996 4.09 18.0596 2.75 16.3996 2.75H7.59961C5.93961 2.75 4.59961 4.09 4.59961 5.75V18.25C4.59961 19.91 5.93961 21.25 7.59961 21.25Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M14 22.25H10C6.7 22.25 4.71 21.59 4.34 18.24C4.28 17.79 4.25 17.25 4.25 16.5V7.5C4.25 6.75 4.28 6.2 4.35 5.73C4.71 2.41 6.7 1.75 10 1.75H14C17.3 1.75 19.29 2.41 19.66 5.76C19.72 6.21 19.75 6.75 19.75 7.5V16.5C19.75 17.25 19.72 17.8 19.65 18.27C19.29 21.59 17.3 22.25 14 22.25ZM10 3.25C6.69 3.25 6.06 3.92 5.83 5.92C5.78 6.34 5.75 6.82 5.75 7.5V16.5C5.75 17.18 5.78 17.66 5.83 18.05C6.05 20.08 6.69 20.75 10 20.75H14C17.31 20.75 17.94 20.08 18.17 18.08C18.23 17.66 18.25 17.18 18.25 16.5V7.5C18.25 6.82 18.22 6.34 18.17 5.95C17.95 3.92 17.31 3.25 14 3.25H10Z" fill="{color}"/>
<path d="M2 20.25C1.59 20.25 1.25 19.91 1.25 19.5V4.5C1.25 4.09 1.59 3.75 2 3.75C2.41 3.75 2.75 4.09 2.75 4.5V19.5C2.75 19.91 2.41 20.25 2 20.25Z" fill="{color}"/>
<path d="M22 19.75C21.59 19.75 21.25 19.41 21.25 19V4C21.25 3.59 21.59 3.25 22 3.25C22.41 3.25 22.75 3.59 22.75 4V19C22.75 19.41 22.41 19.75 22 19.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5 16.5V7.5C5 6.88 5.02 6.33 5.09 5.84C5.38 3.21 6.62 2.5 10 2.5H14C17.38 2.5 18.62 3.21 18.91 5.84C18.98 6.33 19 6.88 19 7.5V16.5C19 17.12 18.98 17.67 18.91 18.16C18.62 20.79 17.38 21.5 14 21.5H10C6.62 21.5 5.38 20.79 5.09 18.16C5.02 17.67 5 17.12 5 16.5Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M2 19.5V4.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M22 19V4" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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