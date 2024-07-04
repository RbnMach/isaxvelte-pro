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
<path d="M12 12L8.8 8.80005L5.5 12L8.8 15.2L15.2 8.80005L18.5 12L15.2 15.2L12 12Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM17.79 12.71L15.95 14.55C15.56 14.94 14.93 14.94 14.54 14.55L12 12L9.45999 14.54C9.06999 14.93 8.43999 14.93 8.04999 14.54L6.20999 12.7C5.81999 12.31 5.81999 11.68 6.20999 11.29L8.04999 9.45C8.43999 9.06 9.06999 9.06 9.45999 9.45L12 12L14.54 9.46001C14.93 9.07001 15.56 9.07001 15.95 9.46001L17.79 11.3C18.18 11.68 18.18 12.32 17.79 12.71Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 12L8.75 8.75L5.5 12L8.75 15.25L15.25 8.75L18.5 12L15.25 15.25L12 12Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.2 2.30001 7.97 2.85001" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M16.001 16l-3.387-3.387c-0.52-0.52-1.36-0.52-1.88 0l-2.453 2.453c-0.52 0.52-0.52 1.36 0 1.88l2.453 2.453c0.52 0.52 1.36 0.52 1.88 0l6.787-6.787c0.52-0.52 1.36-0.52 1.88 0l2.453 2.453c0.52 0.52 0.52 1.36 0 1.88l-2.453 2.453c-0.52 0.52-1.36 0.52-1.88 0l-3.4-3.4z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15.2504 15.9999C15.0604 15.9999 14.8704 15.9299 14.7204 15.7799L12.0004 13.0599L9.28043 15.7799C8.99043 16.0699 8.51043 16.0699 8.22043 15.7799L4.97043 12.5299C4.68043 12.2399 4.68043 11.7599 4.97043 11.4699L8.22043 8.21994C8.51043 7.92994 8.99043 7.92994 9.28043 8.21994L12.0004 10.9399L14.7204 8.21994C15.0104 7.92994 15.4904 7.92994 15.7804 8.21994L19.0304 11.4699C19.3204 11.7599 19.3204 12.2399 19.0304 12.5299L15.7804 15.7799C15.6304 15.9299 15.4404 15.9999 15.2504 15.9999ZM13.0604 11.9999L15.2504 14.1899L17.4404 11.9999L15.2504 9.80994L13.0604 11.9999ZM6.56043 11.9999L8.75043 14.1899L10.9404 11.9999L8.75043 9.80994L6.56043 11.9999Z" fill="{color}"/>
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M12 12L8.75 8.75L5.5 12L8.75 15.25L15.25 8.75L18.5 12L15.25 15.25L12 12Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
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