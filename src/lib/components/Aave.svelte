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
<path d="M8 16L12 7L16 16" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8 12H12" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM16.3 16.69C16.2 16.73 16.1 16.75 16 16.75C15.71 16.75 15.44 16.58 15.31 16.3L12 8.85L10.93 11.25H12C12.41 11.25 12.75 11.59 12.75 12C12.75 12.41 12.41 12.75 12 12.75H10.27L8.69 16.3C8.52 16.68 8.07001 16.85 7.70001 16.68C7.32001 16.51 7.15001 16.07 7.32001 15.69L8.63 12.74H8C7.59 12.74 7.25 12.4 7.25 11.99C7.25 11.58 7.59 11.24 8 11.24H9.28998L11.31 6.69C11.55 6.15 12.44 6.15 12.68 6.69L16.68 15.69C16.85 16.07 16.68 16.52 16.3 16.69Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M8 16L12 7L16 16" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8 12H12" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.19997 2.3 7.96997 2.85" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M22.253 20.933l-5.333-12c-0.32-0.72-1.507-0.72-1.827 0l-2.693 6.067h-1.733c-0.547 0-1 0.453-1 1s0.453 1 1 1h0.827l-1.747 3.933c-0.227 0.507 0 1.093 0.507 1.32s1.093 0 1.32-0.507l2.107-4.733h2.32c0.547 0 1-0.453 1-1s-0.453-1-1-1h-1.427l1.427-3.2 4.413 9.947c0.16 0.373 0.533 0.6 0.92 0.6 0.133 0 0.28-0.027 0.4-0.080 0.507-0.253 0.733-0.853 0.52-1.347z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15.9998 16.7499C15.7098 16.7499 15.4398 16.5799 15.3098 16.2999L11.9998 8.84992L8.68984 16.3099C8.51984 16.6899 8.06985 16.8599 7.69985 16.6899C7.31985 16.5199 7.14985 16.0799 7.31985 15.6999L11.3198 6.69992C11.5598 6.15992 12.4498 6.15992 12.6898 6.69992L16.6898 15.6999C16.8598 16.0799 16.6898 16.5199 16.3098 16.6899C16.2098 16.7299 16.0998 16.7499 15.9998 16.7499Z" fill="{color}"/>
<path d="M12 12.75H8C7.59 12.75 7.25 12.41 7.25 12C7.25 11.59 7.59 11.25 8 11.25H12C12.41 11.25 12.75 11.59 12.75 12C12.75 12.41 12.41 12.75 12 12.75Z" fill="{color}"/>
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<g opacity="0.4">
<path d="M8 16L12 7L16 16" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8 12H12" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</g>
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