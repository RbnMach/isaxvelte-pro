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
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8 7V17H12C14.8 17 17 14.8 17 12C17 9.2 14.8 7 12 7H8Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6.5 10H18.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6.5 14H18.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 7.75H8.75V9.25H15.21C14.43 8.34 13.29 7.75 12 7.75Z" fill="{color}"/>
<path d="M16.25 12C16.25 11.56 16.16 11.15 16.04 10.75H8.75V13.25H16.04C16.16 12.85 16.25 12.44 16.25 12Z" fill="{color}"/>
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM18.52 14.75H17.05C16.07 16.54 14.18 17.75 12 17.75H8C7.59 17.75 7.25 17.41 7.25 17V14.75H6.47998C6.06998 14.75 5.72998 14.41 5.72998 14C5.72998 13.59 6.06998 13.25 6.47998 13.25H7.25V10.75H6.47998C6.06998 10.75 5.72998 10.41 5.72998 10C5.72998 9.59 6.06998 9.25 6.47998 9.25H7.25V7C7.25 6.59 7.59 6.25 8 6.25H12C14.18 6.25 16.07 7.46 17.05 9.25H18.52C18.93 9.25 19.27 9.59 19.27 10C19.27 10.41 18.93 10.75 18.52 10.75H17.61C17.7 11.15 17.75 11.57 17.75 12C17.75 12.43 17.7 12.85 17.61 13.25H18.52C18.93 13.25 19.27 13.59 19.27 14C19.27 14.41 18.93 14.75 18.52 14.75Z" fill="{color}"/>
<path d="M8.75 16.25H12C13.29 16.25 14.43 15.66 15.21 14.75H8.75V16.25Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M8 7V17H12C14.76 17 17 14.76 17 12C17 9.24 14.76 7 12 7H8Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6.48047 10H18.5205" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6.48047 14H18.5205" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.19997 2.3 7.96997 2.85" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M16 23.667h-5.333c-0.547 0-1-0.453-1-1v-13.333c0-0.547 0.453-1 1-1h5.333c4.227 0 7.667 3.44 7.667 7.667s-3.44 7.667-7.667 7.667zM11.667 21.667h4.333c3.12 0 5.667-2.547 5.667-5.667s-2.547-5.667-5.667-5.667h-4.333v11.333z"></path>
<path fill="{color}" d="M24.694 14.333h-16.053c-0.547 0-1-0.453-1-1s0.453-1 1-1h16.053c0.547 0 1 0.453 1 1s-0.453 1-1 1z"></path>
<path fill="{color}" d="M24.694 19.667h-16.053c-0.547 0-1-0.453-1-1s0.453-1 1-1h16.053c0.547 0 1 0.453 1 1s-0.453 1-1 1z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
<path d="M12 17.75H8C7.59 17.75 7.25 17.41 7.25 17V7C7.25 6.59 7.59 6.25 8 6.25H12C15.17 6.25 17.75 8.83 17.75 12C17.75 15.17 15.17 17.75 12 17.75ZM8.75 16.25H12C14.34 16.25 16.25 14.34 16.25 12C16.25 9.66 14.34 7.75 12 7.75H8.75V16.25Z" fill="{color}"/>
<path d="M18.5205 10.75H6.48047C6.07047 10.75 5.73047 10.41 5.73047 10C5.73047 9.59 6.07047 9.25 6.48047 9.25H18.5205C18.9305 9.25 19.2705 9.59 19.2705 10C19.2705 10.41 18.9305 10.75 18.5205 10.75Z" fill="{color}"/>
<path d="M18.5205 14.75H6.48047C6.07047 14.75 5.73047 14.41 5.73047 14C5.73047 13.59 6.07047 13.25 6.48047 13.25H18.5205C18.9305 13.25 19.2705 13.59 19.2705 14C19.2705 14.41 18.9305 14.75 18.5205 14.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<g opacity="0.4">
<path d="M8 7V17H12C14.76 17 17 14.76 17 12C17 9.24 14.76 7 12 7H8Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6.48047 10H18.5205" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6.48047 14H18.5205" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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