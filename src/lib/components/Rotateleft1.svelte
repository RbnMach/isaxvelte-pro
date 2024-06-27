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
<path d="M7.25 22H11.75C15.5 22 17 20.5 17 16.75V12.25C17 8.5 15.5 7 11.75 7H7.25C3.5 7 2 8.5 2 12.25V16.75C2 20.5 3.5 22 7.25 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M22 9C22 5.13 18.87 2 15 2L16.05 3.75" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M7.25 22H11.75C15.5 22 17 20.5 17 16.75V12.25C17 8.5 15.5 7 11.75 7H7.25C3.5 7 2 8.5 2 12.25V16.75C2 20.5 3.5 22 7.25 22Z" fill="{color}"/>
<path d="M21.2504 10.5C20.8404 10.5 20.5004 10.16 20.5004 9.75C20.5004 6.79 18.4404 4.31 15.6704 3.66L15.9404 4.11C16.1504 4.47 16.0404 4.93 15.6804 5.14C15.3204 5.35 14.8604 5.24 14.6504 4.88L13.6004 3.13C13.4604 2.9 13.4604 2.61 13.5904 2.38C13.7304 2.15 13.9804 2 14.2504 2C18.5204 2 22.0004 5.48 22.0004 9.75C22.0004 10.16 21.6604 10.5 21.2504 10.5Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2 16.75C2 20.5 3.5 22 7.25 22H11.75C15.5 22 17 20.5 17 16.75V12.25C17 8.5 15.5 7 11.75 7H7.25C3.5 7 2 8.5 2 12.25" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M22 9C22 5.13 18.87 2 15 2L16.05 3.75" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M7.25 22H11.75C15.5 22 17 20.5 17 16.75V12.25C17 8.5 15.5 7 11.75 7H7.25C3.5 7 2 8.5 2 12.25V16.75C2 20.5 3.5 22 7.25 22Z" fill="{color}"/>
<path d="M21.2504 10.5C20.8404 10.5 20.5004 10.16 20.5004 9.75C20.5004 6.79 18.4404 4.31 15.6704 3.66L15.9404 4.11C16.1504 4.47 16.0404 4.93 15.6804 5.14C15.3204 5.35 14.8604 5.24 14.6504 4.88L13.6004 3.13C13.4604 2.9 13.4604 2.61 13.5904 2.38C13.7304 2.15 13.9804 2 14.2504 2C18.5204 2 22.0004 5.48 22.0004 9.75C22.0004 10.16 21.6604 10.5 21.2504 10.5Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11.75 22.75H7.25C3.1 22.75 1.25 20.9 1.25 16.75V12.25C1.25 8.1 3.1 6.25 7.25 6.25H11.75C15.9 6.25 17.75 8.1 17.75 12.25V16.75C17.75 20.9 15.9 22.75 11.75 22.75ZM7.25 7.75C3.93 7.75 2.75 8.93 2.75 12.25V16.75C2.75 20.07 3.93 21.25 7.25 21.25H11.75C15.07 21.25 16.25 20.07 16.25 16.75V12.25C16.25 8.93 15.07 7.75 11.75 7.75H7.25Z" fill="{color}"/>
<path d="M22.0004 9.75C21.5904 9.75 21.2504 9.41 21.2504 9C21.2504 6.04 19.1904 3.56 16.4204 2.91L16.6904 3.36C16.9004 3.72 16.7904 4.18 16.4304 4.39C16.0704 4.6 15.6104 4.49 15.4004 4.13L14.3504 2.38C14.2104 2.15 14.2104 1.86 14.3404 1.63C14.4804 1.4 14.7304 1.25 15.0004 1.25C19.2704 1.25 22.7504 4.73 22.7504 9C22.7504 9.41 22.4104 9.75 22.0004 9.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M7.25 22H11.75C15.5 22 17 20.5 17 16.75V12.25C17 8.5 15.5 7 11.75 7H7.25C3.5 7 2 8.5 2 12.25V16.75C2 20.5 3.5 22 7.25 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M22 9C22 5.13 18.87 2 15 2L16.05 3.75" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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