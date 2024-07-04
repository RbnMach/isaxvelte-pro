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
<path d="M15 16C18.866 16 22 12.866 22 9C22 5.13401 18.866 2 15 2C11.134 2 8 5.13401 8 9C8 12.866 11.134 16 15 16Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path d="M9 22C12.866 22 16 18.866 16 15C16 11.134 12.866 8 9 8C5.13401 8 2 11.134 2 15C2 18.866 5.13401 22 9 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M9 22C12.866 22 16 18.866 16 15C16 11.134 12.866 8 9 8C5.13401 8 2 11.134 2 15C2 18.866 5.13401 22 9 22Z" fill="{color}"/>
<path d="M21.9998 9C21.9998 11.74 20.4299 14.11 18.1399 15.25C17.8299 15.41 17.4798 15.16 17.4498 14.82C17.1098 10.37 13.5998 6.89 9.17983 6.55C8.82983 6.52 8.58984 6.17 8.74984 5.86C9.88984 3.57 12.2598 2 14.9998 2C18.8698 2 21.9998 5.13 21.9998 9Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15 16C18.866 16 22 12.866 22 9C22 5.13401 18.866 2 15 2C11.134 2 8 5.13401 8 9C8 12.866 11.134 16 15 16Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path d="M5.09003 9.2C6.21003 8.45 7.55 8 9 8C12.87 8 16 11.13 16 15C16 18.87 12.87 22 9 22C5.13 22 2 18.87 2 15C2 14.29 2.09999 13.61 2.29999 12.97" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M20 21.333c5.155 0 9.333-4.179 9.333-9.333s-4.179-9.333-9.333-9.333c-5.155 0-9.333 4.179-9.333 9.333s4.179 9.333 9.333 9.333z"></path>
<path fill="{color}" d="M12 29.333c5.155 0 9.333-4.179 9.333-9.333s-4.179-9.333-9.333-9.333c-5.155 0-9.333 4.179-9.333 9.333s4.179 9.333 9.333 9.333z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15 16.75C10.73 16.75 7.25 13.27 7.25 9C7.25 4.73 10.73 1.25 15 1.25C19.27 1.25 22.75 4.73 22.75 9C22.75 13.27 19.27 16.75 15 16.75ZM15 2.75C11.55 2.75 8.75 5.55 8.75 9C8.75 12.45 11.55 15.25 15 15.25C18.45 15.25 21.25 12.45 21.25 9C21.25 5.55 18.45 2.75 15 2.75Z" fill="{color}"/>
<path d="M9 22.75C4.73 22.75 1.25 19.27 1.25 15C1.25 10.73 4.73 7.25 9 7.25C13.27 7.25 16.75 10.73 16.75 15C16.75 19.27 13.27 22.75 9 22.75ZM9 8.75C5.55 8.75 2.75 11.55 2.75 15C2.75 18.45 5.55 21.25 9 21.25C12.45 21.25 15.25 18.45 15.25 15C15.25 11.55 12.45 8.75 9 8.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M15 16C18.866 16 22 12.866 22 9C22 5.13401 18.866 2 15 2C11.134 2 8 5.13401 8 9C8 12.866 11.134 16 15 16Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path d="M9 22C12.866 22 16 18.866 16 15C16 11.134 12.866 8 9 8C5.13401 8 2 11.134 2 15C2 18.866 5.13401 22 9 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
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