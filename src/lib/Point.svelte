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
<path d="M12 11.5C13.1046 11.5 14 10.6046 14 9.5C14 8.39543 13.1046 7.5 12 7.5C10.8954 7.5 10 8.39543 10 9.5C10 10.6046 10.8954 11.5 12 11.5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path d="M10 13.5C11.3 14.1 12.7 14.1 14 13.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10 16.5L12 14L14 16.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM12 7.12C13.31 7.12 14.38 8.19 14.38 9.5C14.38 10.81 13.31 11.88 12 11.88C10.69 11.88 9.62 10.81 9.62 9.5C9.62 8.19 10.69 7.12 12 7.12ZM14.47 17.09C14.33 17.2 14.17 17.25 14.01 17.25C13.79 17.25 13.57 17.15 13.42 16.97L12.01 15.19L10.6 16.97C10.35 17.29 9.86999 17.35 9.54999 17.09C9.22999 16.83 9.16999 16.36 9.42999 16.04L10.62 14.53C10.3 14.44 9.97999 14.33 9.67999 14.18C9.30999 13.99 9.15998 13.54 9.34998 13.17C9.52998 12.8 9.97999 12.65 10.36 12.84C11.4 13.36 12.64 13.36 13.68 12.84C14.04 12.66 14.5 12.8 14.68 13.16C14.87 13.52 14.74 13.97 14.38 14.16C14.07 14.32 13.74 14.43 13.41 14.52L14.61 16.03C14.84 16.36 14.79 16.83 14.47 17.09Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 11.5C13.1046 11.5 14 10.6046 14 9.5C14 8.39543 13.1046 7.5 12 7.5C10.8954 7.5 10 8.39543 10 9.5C10 10.6046 10.8954 11.5 12 11.5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path d="M10 13.5C11.25 14.13 12.73 14.13 13.99 13.51L14 13.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10 16.5L12 13.97L14 16.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M15.999 15.84c1.753 0 3.173-1.421 3.173-3.173s-1.421-3.173-3.173-3.173c-1.753 0-3.173 1.421-3.173 3.173s1.421 3.173 3.173 3.173z"></path>
<path fill="{color}" d="M19.454 21.374l-1.6-2.013c0.44-0.12 0.88-0.28 1.293-0.48 0.48-0.267 0.653-0.853 0.4-1.333s-0.853-0.667-1.333-0.427c-1.387 0.693-3.040 0.693-4.427 0-0.493-0.253-1.093-0.053-1.347 0.44s-0.053 1.093 0.44 1.347c0.4 0.2 0.827 0.36 1.253 0.467l-1.587 2.013c-0.347 0.44-0.267 1.067 0.16 1.4 0.44 0.347 1.067 0.267 1.4-0.16l1.88-2.373 1.88 2.373c0.2 0.253 0.493 0.373 0.787 0.373 0.213 0 0.44-0.067 0.613-0.213 0.453-0.347 0.52-0.973 0.187-1.413z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 12.25C10.48 12.25 9.25 11.02 9.25 9.5C9.25 7.98 10.48 6.75 12 6.75C13.52 6.75 14.75 7.98 14.75 9.5C14.75 11.02 13.52 12.25 12 12.25ZM12 8.25C11.31 8.25 10.75 8.81 10.75 9.5C10.75 10.19 11.31 10.75 12 10.75C12.69 10.75 13.25 10.19 13.25 9.5C13.25 8.81 12.69 8.25 12 8.25Z" fill="{color}"/>
<path d="M11.9905 14.72C11.1905 14.72 10.3905 14.54 9.66048 14.17C9.29048 13.98 9.14052 13.53 9.33052 13.16C9.51052 12.79 9.96053 12.64 10.3405 12.83C11.3805 13.35 12.6205 13.35 13.6605 12.83C14.0205 12.65 14.4805 12.79 14.6605 13.15C14.8505 13.51 14.7205 13.96 14.3605 14.15C13.6105 14.53 12.8005 14.72 11.9905 14.72Z" fill="{color}"/>
<path d="M13.9996 17.2502C13.7796 17.2502 13.5595 17.1502 13.4095 16.9702L11.9996 15.1902L10.5896 16.9702C10.3396 17.2902 9.85954 17.3502 9.53954 17.0902C9.21954 16.8302 9.15955 16.3602 9.41955 16.0402L11.4195 13.5102C11.6995 13.1502 12.3095 13.1502 12.5995 13.5102L14.5995 16.0402C14.8595 16.3702 14.7995 16.8402 14.4795 17.0902C14.3295 17.2002 14.1596 17.2502 13.9996 17.2502Z" fill="{color}"/>
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<g opacity="0.4">
<path d="M12 11.5C13.1046 11.5 14 10.6046 14 9.5C14 8.39543 13.1046 7.5 12 7.5C10.8954 7.5 10 8.39543 10 9.5C10 10.6046 10.8954 11.5 12 11.5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path d="M10 13.5C11.25 14.13 12.73 14.13 13.99 13.51L14 13.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10 16.4997L12 13.9697L14 16.4997" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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