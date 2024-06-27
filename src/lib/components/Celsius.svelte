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
<path d="M16.3001 15.3001C15.3001 16.6001 13.7001 17.5001 12.0001 17.5001C9.0001 17.5001 6.6001 15.1001 6.6001 12.1001C6.6001 9.1001 9.0001 6.6001 12.0001 6.6001C13.2001 6.6001 14.4001 7.0001 15.3001 7.7001" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17.4 11.4C18.0627 11.4 18.6 10.8627 18.6 10.2C18.6 9.53726 18.0627 9 17.4 9C16.7372 9 16.2 9.53726 16.2 10.2C16.2 10.8627 16.7372 11.4 17.4 11.4Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM16.93 15.74C15.75 17.3 13.95 18.19 12 18.19C8.59 18.19 5.81 15.41 5.81 12C5.81 8.59 8.59 5.81 12 5.81C13.35 5.81 14.64 6.24 15.72 7.05C16.05 7.3 16.12 7.77001 15.87 8.10001C15.62 8.43001 15.15 8.5 14.82 8.25C14 7.63 13.03 7.31 12 7.31C9.42 7.31 7.31 9.41 7.31 12C7.31 14.59 9.41 16.69 12 16.69C13.48 16.69 14.84 16.01 15.74 14.83C15.99 14.5 16.46 14.44 16.79 14.69C17.12 14.94 17.18 15.41 16.93 15.74ZM17.42 11.34C16.77 11.34 16.25 10.82 16.25 10.17C16.25 9.52 16.77 9 17.42 9C18.07 9 18.59 9.52 18.59 10.17C18.59 10.82 18.07 11.34 17.42 11.34Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.3306 15.28C15.3406 16.59 13.7605 17.43 12.0005 17.43C9.00055 17.43 6.56055 15.0001 6.56055 11.9901C6.56055 8.98005 8.99055 6.55005 12.0005 6.55005C13.2305 6.55005 14.3606 6.96005 15.2706 7.64005" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17.42 11.34C18.0662 11.34 18.59 10.8162 18.59 10.17C18.59 9.52382 18.0662 9 17.42 9C16.7738 9 16.25 9.52382 16.25 10.17C16.25 10.8162 16.7738 11.34 17.42 11.34Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.2 2.30001 7.97 2.85001" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M16.001 24.253c-4.547 0-8.253-3.707-8.253-8.253s3.707-8.253 8.253-8.253c1.8 0 3.52 0.573 4.96 1.653 0.44 0.333 0.533 0.96 0.2 1.4s-0.96 0.533-1.4 0.2c-1.093-0.813-2.387-1.253-3.76-1.253-3.44 0-6.253 2.8-6.253 6.253s2.8 6.253 6.253 6.253c1.973 0 3.787-0.907 4.987-2.48 0.333-0.44 0.96-0.52 1.4-0.187s0.52 0.96 0.187 1.4c-1.573 2.067-3.973 3.267-6.573 3.267z"></path>
<path fill="{color}" d="M23.227 15.12c0.862 0 1.56-0.698 1.56-1.56s-0.698-1.56-1.56-1.56-1.56 0.698-1.56 1.56c0 0.862 0.698 1.56 1.56 1.56z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11.9996 18.1901C8.58957 18.1901 5.80957 15.4101 5.80957 12.0001C5.80957 8.59006 8.58957 5.81006 11.9996 5.81006C13.3496 5.81006 14.6396 6.24006 15.7196 7.05006C16.0496 7.30006 16.1196 7.77007 15.8696 8.10007C15.6196 8.43007 15.1496 8.50006 14.8196 8.25006C13.9996 7.63006 13.0296 7.31006 11.9996 7.31006C9.41957 7.31006 7.30957 9.41006 7.30957 12.0001C7.30957 14.5901 9.40957 16.6901 11.9996 16.6901C13.4796 16.6901 14.8396 16.0101 15.7396 14.8301C15.9896 14.5001 16.4596 14.4401 16.7896 14.6901C17.1196 14.9401 17.1796 15.4101 16.9296 15.7401C15.7496 17.2901 13.9496 18.1901 11.9996 18.1901Z" fill="{color}"/>
<path d="M17.42 12.09C16.36 12.09 15.5 11.23 15.5 10.17C15.5 9.11 16.36 8.25 17.42 8.25C18.48 8.25 19.34 9.11 19.34 10.17C19.34 11.23 18.48 12.09 17.42 12.09ZM17.42 9.75C17.19 9.75 17 9.94 17 10.17C17 10.4 17.19 10.59 17.42 10.59C17.65 10.59 17.84 10.4 17.84 10.17C17.84 9.94 17.65 9.75 17.42 9.75Z" fill="{color}"/>
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M16.3296 15.2798C15.3396 16.5898 13.7596 17.4298 11.9996 17.4298C8.99957 17.4298 6.55957 14.9998 6.55957 11.9898C6.55957 8.97981 8.98957 6.5498 11.9996 6.5498C13.2296 6.5498 14.3596 6.9598 15.2696 7.6398" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M17.42 11.34C18.0662 11.34 18.59 10.8162 18.59 10.17C18.59 9.52382 18.0662 9 17.42 9C16.7738 9 16.25 9.52382 16.25 10.17C16.25 10.8162 16.7738 11.34 17.42 11.34Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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