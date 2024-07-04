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
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.8 8H10.8C9.20005 8 7.80005 9.4 7.80005 11V12V13C7.80005 14.6 9.20005 16 10.8 16H15.8" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.8 12H7.80005" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM15.75 11.25C16.16 11.25 16.5 11.59 16.5 12C16.5 12.41 16.16 12.75 15.75 12.75H8.5V13C8.5 14.24 9.51 15.25 10.75 15.25H15.75C16.16 15.25 16.5 15.59 16.5 16C16.5 16.41 16.16 16.75 15.75 16.75H10.75C8.68 16.75 7 15.07 7 13V11C7 8.93 8.68 7.25 10.75 7.25H15.75C16.16 7.25 16.5 7.59 16.5 8C16.5 8.41 16.16 8.75 15.75 8.75H10.75C9.51 8.75 8.5 9.76 8.5 11V11.25H15.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15.75 8H10.75C9.1 8 7.75 9.35 7.75 11V12V13C7.75 14.65 9.1 16 10.75 16H15.75" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.75 12H7.75" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.2 2.30001 7.97 2.85001" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M21 17c0.547 0 1-0.453 1-1s-0.453-1-1-1h-9.667v-0.333c0-1.653 1.347-3 3-3h6.667c0.547 0 1-0.453 1-1s-0.453-1-1-1h-6.667c-2.76 0-5 2.24-5 5v2.667c0 2.76 2.24 5 5 5h6.667c0.547 0 1-0.453 1-1s-0.453-1-1-1h-6.667c-1.653 0-3-1.347-3-3v-0.333h9.667z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
<path d="M15.75 16.75H10.75C8.68 16.75 7 15.07 7 13V11C7 8.93 8.68 7.25 10.75 7.25H15.75C16.16 7.25 16.5 7.59 16.5 8C16.5 8.41 16.16 8.75 15.75 8.75H10.75C9.51 8.75 8.5 9.76 8.5 11V13C8.5 14.24 9.51 15.25 10.75 15.25H15.75C16.16 15.25 16.5 15.59 16.5 16C16.5 16.41 16.16 16.75 15.75 16.75Z" fill="{color}"/>
<path d="M15.75 12.75H7.75C7.34 12.75 7 12.41 7 12C7 11.59 7.34 11.25 7.75 11.25H15.75C16.16 11.25 16.5 11.59 16.5 12C16.5 12.41 16.16 12.75 15.75 12.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<g opacity="0.4">
<path d="M15.75 8H10.75C9.1 8 7.75 9.35 7.75 11V12V13C7.75 14.65 9.1 16 10.75 16H15.75" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.75 12H7.75" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</g>
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