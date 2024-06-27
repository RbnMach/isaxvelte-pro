<script lang="ts">
	export let classes = '';
	export let color = 'currentColor';
	export let type: 'linear' | 'bold' | 'broken' | 'bulk' | 'outline' | 'twotone' = 'linear';
	export let size = '1em';
	export let axis_y = '-0.13em';
	export let axis_x = '0';
</script>

<span style="width: {size}; height: {size}; bottom: {axis_y}; left: {axis_x};" class={classes}>
	{#if type == 'linear'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path d="M9 11L11.5 6H12.5L15 11" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8 13L7 15L12 18L17 15L16 13" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM8.33 10.66L10.83 5.66C10.96 5.41 11.22 5.25 11.5 5.25H12.5C12.78 5.25 13.04 5.41 13.17 5.66L15.67 10.66C15.86 11.03 15.71 11.48 15.33 11.67C15.22 11.72 15.11 11.75 15 11.75C14.73 11.75 14.46 11.6 14.33 11.34L12.04 6.75H11.97L9.68 11.34C9.5 11.71 9.05 11.86 8.67 11.68C8.29 11.49 8.14 11.04 8.33 10.66ZM17.39 15.64L12.39 18.64C12.27 18.71 12.14 18.75 12 18.75C11.86 18.75 11.73 18.71 11.61 18.64L6.61 15.64C6.27 15.44 6.15 15.01 6.32 14.66L7.32 12.66C7.51 12.29 7.96 12.14 8.33 12.32C8.7 12.51 8.85 12.96 8.67 13.33L7.98 14.71L12 17.12L16.02 14.71L15.33 13.33C15.14 12.96 15.29 12.51 15.67 12.32C16.04 12.14 16.49 12.28 16.68 12.66L17.68 14.66C17.85 15.01 17.72 15.44 17.39 15.64Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M9 11L11.5 6H12.5L15 11" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8 13L7 15L12 18L17 15L16 13" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.2 2.30001 7.97 2.85001" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M20 15.666c-0.36 0-0.72-0.2-0.893-0.547l-3.053-6.12h-0.093l-3.053 6.12c-0.24 0.493-0.84 0.693-1.347 0.453-0.493-0.253-0.693-0.853-0.453-1.347l3.333-6.667c0.173-0.333 0.52-0.547 0.893-0.547h1.333c0.373 0 0.72 0.213 0.893 0.547l3.333 6.667c0.253 0.493 0.053 1.093-0.453 1.347-0.133 0.053-0.293 0.093-0.44 0.093z"></path>
<path fill="{color}" d="M16.001 25c-0.173 0-0.36-0.053-0.52-0.147l-6.667-4c-0.453-0.267-0.613-0.84-0.387-1.307l1.333-2.667c0.253-0.493 0.853-0.693 1.347-0.453 0.493 0.253 0.693 0.853 0.453 1.347l-0.92 1.84 5.36 3.213 5.36-3.213-0.92-1.84c-0.253-0.493-0.053-1.093 0.453-1.347 0.493-0.24 1.093-0.053 1.347 0.453l1.333 2.667c0.24 0.467 0.067 1.040-0.387 1.307l-6.667 4c-0.16 0.093-0.347 0.147-0.52 0.147z"></path>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
<path d="M14.9999 11.7498C14.7299 11.7498 14.4599 11.5998 14.3299 11.3398L12.0399 6.74977H11.9699L9.67994 11.3398C9.49994 11.7098 9.04994 11.8598 8.66994 11.6798C8.29994 11.4898 8.14994 11.0398 8.32994 10.6698L10.8299 5.66977C10.9599 5.41977 11.2199 5.25977 11.4999 5.25977H12.4999C12.7799 5.25977 13.0399 5.41977 13.1699 5.66977L15.6699 10.6698C15.8599 11.0398 15.7099 11.4898 15.3299 11.6798C15.2299 11.7198 15.1099 11.7498 14.9999 11.7498Z" fill="{color}"/>
<path d="M11.9998 18.75C11.8698 18.75 11.7298 18.71 11.6098 18.64L6.60977 15.64C6.26977 15.44 6.14977 15.01 6.31977 14.66L7.31977 12.66C7.50977 12.29 7.95977 12.14 8.32977 12.32C8.69977 12.51 8.84977 12.96 8.66977 13.33L7.97977 14.71L11.9998 17.12L16.0198 14.71L15.3298 13.33C15.1398 12.96 15.2898 12.51 15.6698 12.32C16.0398 12.14 16.4898 12.28 16.6798 12.66L17.6798 14.66C17.8598 15.01 17.7298 15.44 17.3898 15.64L12.3898 18.64C12.2698 18.71 12.1298 18.75 11.9998 18.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path opacity="0.4" d="M9 11L11.5 6H12.5L15 11" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M8 13L7 15L12 18L17 15L16 13" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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
</style>