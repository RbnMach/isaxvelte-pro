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
<path d="M16.75 22H12.25C8.5 22 7 20.5 7 16.75V12.25C7 8.5 8.5 7 12.25 7H16.75C20.5 7 22 8.5 22 12.25V16.75C22 20.5 20.5 22 16.75 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 9C2 5.13 5.13 2 9 2L7.95 3.75" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.75 22H12.25C8.5 22 7 20.5 7 16.75V12.25C7 8.5 8.5 7 12.25 7H16.75C20.5 7 22 8.5 22 12.25V16.75C22 20.5 20.5 22 16.75 22Z" fill="{color}"/>
<path d="M2.75 10.5C3.16 10.5 3.5 10.16 3.5 9.75C3.5 6.79 5.56 4.31 8.33 3.66L8.06 4.11C7.85 4.47 7.96 4.93 8.32 5.14C8.68 5.35 9.14 5.24 9.35 4.88L10.4 3.13C10.54 2.9 10.54 2.61 10.41 2.38C10.27 2.15 10.02 2 9.75 2C5.48 2 2 5.48 2 9.75C2 10.16 2.34 10.5 2.75 10.5Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M22 16.75C22 20.5 20.5 22 16.75 22H12.25C8.5 22 7 20.5 7 16.75V12.25C7 8.5 8.5 7 12.25 7H16.75C20.5 7 22 8.5 22 12.25" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 9C2 5.13 5.13 2 9 2L7.95 3.75" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M16.75 22H12.25C8.5 22 7 20.5 7 16.75V12.25C7 8.5 8.5 7 12.25 7H16.75C20.5 7 22 8.5 22 12.25V16.75C22 20.5 20.5 22 16.75 22Z" fill="{color}"/>
<path d="M2.75 10.5C3.16 10.5 3.5 10.16 3.5 9.75C3.5 6.79 5.56 4.31 8.33 3.66L8.06 4.11C7.85 4.47 7.96 4.93 8.32 5.14C8.68 5.35 9.14 5.24 9.35 4.88L10.4 3.13C10.54 2.9 10.54 2.61 10.41 2.38C10.27 2.15 10.02 2 9.75 2C5.48 2 2 5.48 2 9.75C2 10.16 2.34 10.5 2.75 10.5Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.75 22.75H12.25C8.1 22.75 6.25 20.9 6.25 16.75V12.25C6.25 8.1 8.1 6.25 12.25 6.25H16.75C20.9 6.25 22.75 8.1 22.75 12.25V16.75C22.75 20.9 20.9 22.75 16.75 22.75ZM12.25 7.75C8.93 7.75 7.75 8.93 7.75 12.25V16.75C7.75 20.07 8.93 21.25 12.25 21.25H16.75C20.07 21.25 21.25 20.07 21.25 16.75V12.25C21.25 8.93 20.07 7.75 16.75 7.75H12.25Z" fill="{color}"/>
<path d="M2 9.75C1.59 9.75 1.25 9.41 1.25 9C1.25 4.73 4.73 1.25 9 1.25C9.27 1.25 9.52 1.4 9.65 1.63C9.78 1.86 9.78 2.15 9.64 2.38L8.59 4.14C8.38 4.49 7.92 4.61 7.56 4.39C7.21 4.18 7.09 3.72 7.31 3.36L7.58 2.91C4.81 3.56 2.75 6.04 2.75 9C2.75 9.41 2.41 9.75 2 9.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.75 22H12.25C8.5 22 7 20.5 7 16.75V12.25C7 8.5 8.5 7 12.25 7H16.75C20.5 7 22 8.5 22 12.25V16.75C22 20.5 20.5 22 16.75 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M2 9C2 5.13 5.13 2 9 2L7.95 3.75" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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