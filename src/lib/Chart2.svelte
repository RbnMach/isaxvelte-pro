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
<path d="M7 10.74V13.94" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 9V15.68" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17 10.74V13.94" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9 22H15C20 22 22 20 22 15V9C22 4 20 2 15 2H9C4 2 2 4 2 9V15C2 20 4 22 9 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.19 2H7.81C4.17 2 2 4.17 2 7.81V16.19C2 19.83 4.17 22 7.81 22H16.19C19.83 22 22 19.83 22 16.19V7.81C22 4.17 19.83 2 16.19 2ZM7.75 13.6C7.75 14.01 7.41 14.35 7 14.35C6.59 14.35 6.25 14.01 6.25 13.6V10.4C6.25 9.99 6.59 9.65 7 9.65C7.41 9.65 7.75 9.99 7.75 10.4V13.6ZM12.75 15.34C12.75 15.75 12.41 16.09 12 16.09C11.59 16.09 11.25 15.75 11.25 15.34V8.66C11.25 8.25 11.59 7.91 12 7.91C12.41 7.91 12.75 8.25 12.75 8.66V15.34ZM17.75 13.6C17.75 14.01 17.41 14.35 17 14.35C16.59 14.35 16.25 14.01 16.25 13.6V10.4C16.25 9.99 16.59 9.65 17 9.65C17.41 9.65 17.75 9.99 17.75 10.4V13.6Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M7 10.74V13.94" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 15.68V12.76" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 9V10.01" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17 10.74V13.94" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 12.98V15C2 20 4 22 9 22H15C20 22 22 20 22 15V9C22 4 20 2 15 2H9C4 2 2 4 2 9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M16.19 2H7.81C4.17 2 2 4.17 2 7.81V16.18C2 19.83 4.17 22 7.81 22H16.18C19.82 22 21.99 19.83 21.99 16.19V7.81C22 4.17 19.83 2 16.19 2Z" fill="{color}"/>
<path d="M7 14.3499C6.59 14.3499 6.25 14.0099 6.25 13.5999V10.3999C6.25 9.9899 6.59 9.6499 7 9.6499C7.41 9.6499 7.75 9.9899 7.75 10.3999V13.6099C7.75 14.0199 7.41 14.3499 7 14.3499Z" fill="{color}"/>
<path d="M12 16.0902C11.59 16.0902 11.25 15.7502 11.25 15.3402V8.66016C11.25 8.25016 11.59 7.91016 12 7.91016C12.41 7.91016 12.75 8.25016 12.75 8.66016V15.3402C12.75 15.7502 12.41 16.0902 12 16.0902Z" fill="{color}"/>
<path d="M17 14.3499C16.59 14.3499 16.25 14.0099 16.25 13.5999V10.3999C16.25 9.9899 16.59 9.6499 17 9.6499C17.41 9.6499 17.75 9.9899 17.75 10.3999V13.6099C17.75 14.0199 17.41 14.3499 17 14.3499Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M7 14.69C6.59 14.69 6.25 14.35 6.25 13.94V10.73C6.25 10.32 6.59 9.97998 7 9.97998C7.41 9.97998 7.75 10.32 7.75 10.73V13.94C7.75 14.36 7.41 14.69 7 14.69Z" fill="{color}"/>
<path d="M12 16.43C11.59 16.43 11.25 16.09 11.25 15.68V9C11.25 8.59 11.59 8.25 12 8.25C12.41 8.25 12.75 8.59 12.75 9V15.68C12.75 16.09 12.41 16.43 12 16.43Z" fill="{color}"/>
<path d="M17 14.69C16.59 14.69 16.25 14.35 16.25 13.94V10.73C16.25 10.32 16.59 9.97998 17 9.97998C17.41 9.97998 17.75 10.32 17.75 10.73V13.94C17.75 14.36 17.41 14.69 17 14.69Z" fill="{color}"/>
<path d="M15 22.75H9C3.57 22.75 1.25 20.43 1.25 15V9C1.25 3.57 3.57 1.25 9 1.25H15C20.43 1.25 22.75 3.57 22.75 9V15C22.75 20.43 20.43 22.75 15 22.75ZM9 2.75C4.39 2.75 2.75 4.39 2.75 9V15C2.75 19.61 4.39 21.25 9 21.25H15C19.61 21.25 21.25 19.61 21.25 15V9C21.25 4.39 19.61 2.75 15 2.75H9Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<g opacity="0.4">
<path d="M7 10.7402V13.9402" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 9V15.68" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17 10.7402V13.9402" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</g>
<path d="M9 22H15C20 22 22 20 22 15V9C22 4 20 2 15 2H9C4 2 2 4 2 9V15C2 20 4 22 9 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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