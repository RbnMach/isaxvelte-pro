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
<path d="M9.5 8.5L12 11.9L14.5 8.5H9.5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path d="M17 10L12 17L7 10" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM9.04999 8.28999C9.12999 8.11999 9.31 8.00999 9.5 8.00999H14.5C14.69 8.00999 14.86 8.11999 14.95 8.28999C15.04 8.45999 15.02 8.66 14.9 8.81L12.4 12.14C12.31 12.27 12.16 12.34 12 12.34C11.84 12.34 11.69 12.27 11.6 12.14L9.09998 8.81C8.98998 8.67 8.96999 8.45999 9.04999 8.28999ZM17.61 10.44L12.61 17.44C12.47 17.64 12.24 17.75 12 17.75C11.76 17.75 11.53 17.63 11.39 17.44L6.39001 10.44C6.15001 10.1 6.23 9.63 6.56 9.39C6.9 9.15 7.36999 9.23 7.60999 9.56L12 15.71L16.39 9.56C16.63 9.22 17.1 9.14 17.44 9.39C17.77 9.63 17.85 10.1 17.61 10.44Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M9.5 8.52002L12 11.85L14.5 8.52002H9.5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17 10L12 17L7 10" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.19997 2.30001 7.96997 2.85001" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" d="M19.933 11.053c-0.107-0.227-0.347-0.373-0.6-0.373h-6.667c-0.253 0-0.48 0.147-0.6 0.373s-0.093 0.493 0.067 0.693l3.333 4.44c0.12 0.173 0.32 0.267 0.533 0.267s0.413-0.093 0.533-0.267l3.333-4.44c0.147-0.187 0.173-0.467 0.067-0.693z"></path>
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M16.001 23.667c-0.32 0-0.627-0.16-0.813-0.413l-6.667-9.333c-0.32-0.453-0.213-1.080 0.227-1.4 0.453-0.32 1.080-0.213 1.4 0.227l5.853 8.2 5.853-8.2c0.32-0.453 0.947-0.56 1.4-0.227 0.453 0.32 0.56 0.947 0.227 1.4l-6.667 9.333c-0.187 0.253-0.493 0.413-0.813 0.413z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11.9996 12.6C11.7596 12.6 11.5396 12.49 11.3996 12.3L8.89964 8.97002C8.72964 8.74002 8.69963 8.44001 8.82963 8.18001C8.95963 7.92001 9.21962 7.77002 9.49962 7.77002H14.4996C14.7796 7.77002 15.0396 7.93001 15.1696 8.18001C15.2996 8.43001 15.2696 8.74002 15.0996 8.97002L12.5996 12.3C12.4596 12.49 12.2396 12.6 11.9996 12.6ZM10.9996 9.27002L11.9996 10.6L12.9996 9.27002H10.9996Z" fill="{color}"/>
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
<path d="M11.9999 17.7502C11.7599 17.7502 11.5299 17.6302 11.3899 17.4402L6.38992 10.4402C6.14992 10.1002 6.2299 9.63024 6.5599 9.39024C6.8999 9.15024 7.36989 9.23024 7.60989 9.56024L11.9999 15.7102L16.3899 9.56024C16.6299 9.22024 17.0999 9.14024 17.4399 9.39024C17.7799 9.63024 17.8599 10.1002 17.6099 10.4402L12.6099 17.4402C12.4699 17.6302 12.2399 17.7502 11.9999 17.7502Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M9.5 8.52002L12 11.85L14.5 8.52002H9.5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path opacity="0.4" d="M17 10L12 17L7 10" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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