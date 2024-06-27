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
<path d="M2 12H9C10.7 12 12 13.3 12 15C12 16.7 10.7 18 9 18H3C2.4 18 2 17.6 2 17V7C2 6.4 2.4 6 3 6H8C9.7 6 11 7.3 11 9C11 10.7 9.7 12 8 12H2Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path d="M14 14H22C22 11.8 20.2 10 18 10C15.8 10 14 11.8 14 14ZM14 14C14 16.2 15.8 18 18 18H19.7" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M19.5 7.5H16.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M9 18.75H3C2.04 18.75 1.25 17.96 1.25 17V7C1.25 6.04 2.04 5.25 3 5.25H8C10.07 5.25 11.75 6.93 11.75 9C11.75 10.03 11.33 10.96 10.66 11.64C11.9 12.25 12.75 13.53 12.75 15C12.75 17.07 11.07 18.75 9 18.75ZM2.75 12.75V17C2.75 17.14 2.86 17.25 3 17.25H9C10.24 17.25 11.25 16.24 11.25 15C11.25 13.76 10.24 12.75 9 12.75H2.75ZM2.75 11.25H8C9.24 11.25 10.25 10.24 10.25 9C10.25 7.76 9.24 6.75 8 6.75H3C2.86 6.75 2.75 6.86 2.75 7V11.25Z" fill="{color}"/>
<path d="M19.67 18.75H18C15.38 18.75 13.25 16.62 13.25 14C13.25 11.38 15.38 9.25 18 9.25C20.62 9.25 22.75 11.38 22.75 14C22.75 14.41 22.41 14.75 22 14.75H14.84C15.18 16.18 16.47 17.25 18 17.25H19.67C20.08 17.25 20.42 17.59 20.42 18C20.42 18.41 20.08 18.75 19.67 18.75ZM14.84 13.25H21.17C20.83 11.82 19.54 10.75 18.01 10.75C16.48 10.75 15.18 11.82 14.84 13.25Z" fill="{color}"/>
<path d="M19.5 8.25H16.5C16.09 8.25 15.75 7.91 15.75 7.5C15.75 7.09 16.09 6.75 16.5 6.75H19.5C19.91 6.75 20.25 7.09 20.25 7.5C20.25 7.91 19.91 8.25 19.5 8.25Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2 7C2 6.45 2.45 6 3 6H8C9.66 6 11 7.34 11 9C11 10.66 9.66 12 8 12H2H9C10.66 12 12 13.34 12 15C12 16.66 10.66 18 9 18H3C2.45 18 2 17.55 2 17V10.97" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M14 14H22C22 11.79 20.21 10 18 10C15.79 10 14 11.79 14 14ZM14 14C14 16.21 15.79 18 18 18H19.67" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M19.5 7.5H16.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" d="M12 25h-8c-1.28 0-2.333-1.053-2.333-2.333v-13.333c0-1.28 1.053-2.333 2.333-2.333h6.667c2.76 0 5 2.24 5 5 0 1.373-0.56 2.613-1.453 3.52 1.653 0.813 2.787 2.52 2.787 4.48 0 2.76-2.24 5-5 5zM3.667 17v5.667c0 0.187 0.147 0.333 0.333 0.333h8c1.653 0 3-1.347 3-3s-1.347-3-3-3h-8.333zM3.667 15h7c1.653 0 3-1.347 3-3s-1.347-3-3-3h-6.667c-0.187 0-0.333 0.147-0.333 0.333v5.667z"></path>
<path fill="{color}" opacity="0.4" d="M26.227 25h-2.227c-3.493 0-6.333-2.84-6.333-6.333s2.84-6.333 6.333-6.333c3.493 0 6.333 2.84 6.333 6.333 0 0.547-0.453 1-1 1h-9.547c0.453 1.907 2.173 3.333 4.213 3.333h2.227c0.547 0 1 0.453 1 1s-0.453 1-1 1zM19.787 17.667h8.44c-0.453-1.907-2.173-3.333-4.213-3.333s-3.773 1.427-4.227 3.333z"></path>
<path fill="{color}" d="M26 11h-4c-0.547 0-1-0.453-1-1s0.453-1 1-1h4c0.547 0 1 0.453 1 1s-0.453 1-1 1z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M9 18.75H3C2.04 18.75 1.25 17.96 1.25 17V7C1.25 6.04 2.04 5.25 3 5.25H8C10.07 5.25 11.75 6.93 11.75 9C11.75 10.03 11.33 10.96 10.66 11.64C11.9 12.25 12.75 13.53 12.75 15C12.75 17.07 11.07 18.75 9 18.75ZM2.75 12.75V17C2.75 17.14 2.86 17.25 3 17.25H9C10.24 17.25 11.25 16.24 11.25 15C11.25 13.76 10.24 12.75 9 12.75H2.75ZM2.75 11.25H8C9.24 11.25 10.25 10.24 10.25 9C10.25 7.76 9.24 6.75 8 6.75H3C2.86 6.75 2.75 6.86 2.75 7V11.25Z" fill="{color}"/>
<path d="M19.67 18.75H18C15.38 18.75 13.25 16.62 13.25 14C13.25 11.38 15.38 9.25 18 9.25C20.62 9.25 22.75 11.38 22.75 14C22.75 14.41 22.41 14.75 22 14.75H14.84C15.18 16.18 16.47 17.25 18 17.25H19.67C20.08 17.25 20.42 17.59 20.42 18C20.42 18.41 20.08 18.75 19.67 18.75ZM14.84 13.25H21.17C20.83 11.82 19.54 10.75 18.01 10.75C16.48 10.75 15.18 11.82 14.84 13.25Z" fill="{color}"/>
<path d="M19.5 8.25H16.5C16.09 8.25 15.75 7.91 15.75 7.5C15.75 7.09 16.09 6.75 16.5 6.75H19.5C19.91 6.75 20.25 7.09 20.25 7.5C20.25 7.91 19.91 8.25 19.5 8.25Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2 12H9C10.66 12 12 13.34 12 15C12 16.66 10.66 18 9 18H3C2.45 18 2 17.55 2 17V7C2 6.45 2.45 6 3 6H8C9.66 6 11 7.34 11 9C11 10.66 9.66 12 8 12H2Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path opacity="0.4" d="M14 14H22C22 11.79 20.21 10 18 10C15.79 10 14 11.79 14 14ZM14 14C14 16.21 15.79 18 18 18H19.67" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M19.5 7.5H16.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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