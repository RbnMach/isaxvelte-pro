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
<path d="M11 5V8H9C8.4 8 8 8.4 8 9V11H5V9C5 6.8 6.8 5 9 5H11Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M13 19V16H15C15.6 16 16 15.6 16 15V13H19V15C19 17.2 17.2 19 15 19H13Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15 22H9C4 22 2 20 2 15V9C2 4 4 2 9 2H15C20 2 22 4 22 9V15C22 20 20 22 15 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.1898 2H7.81978C4.17978 2 2.00977 4.17 2.00977 7.81V16.18C2.00977 19.82 4.17978 21.99 7.81978 21.99H16.1898C19.8298 21.99 21.9998 19.82 21.9998 16.18V7.81C21.9998 4.17 19.8298 2 16.1898 2ZM10.9998 7.5C10.9998 7.78 10.7798 8 10.4998 8H8.99977C8.44977 8 7.99977 8.45 7.99977 9V10.5C7.99977 10.78 7.77977 11 7.49977 11H5.49977C5.21977 11 4.99977 10.78 4.99977 10.5V9C4.99977 6.79 6.78977 5 8.99977 5H10.4998C10.7798 5 10.9998 5.22 10.9998 5.5V7.5ZM18.9998 15C18.9998 17.21 17.2098 19 14.9998 19H13.4998C13.2198 19 12.9998 18.78 12.9998 18.5V16.5C12.9998 16.22 13.2198 16 13.4998 16H14.9998C15.5498 16 15.9998 15.55 15.9998 15V13.5C15.9998 13.22 16.2198 13 16.4998 13H18.4998C18.7798 13 18.9998 13.22 18.9998 13.5V15Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11 5V8H9C8.45 8 8 8.45 8 9V11H5V9C5 6.79 6.79 5 9 5H11Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M13 19V16H15C15.55 16 16 15.55 16 15V13H19V15C19 17.21 17.21 19 15 19H13Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 12.83V15C2 20 4 22 9 22H15C20 22 22 20 22 15V9C22 4 20 2 15 2H9C4 2 2 4 2 9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M21.586 2.667h-11.16c-4.853 0-7.747 2.893-7.747 7.747v11.16c0 4.853 2.893 7.747 7.747 7.747h11.16c4.853 0 7.747-2.893 7.747-7.747v-11.16c0-4.853-2.893-7.747-7.747-7.747z"></path>
<path fill="{color}" d="M14.667 7.333v2.667c0 0.373-0.293 0.667-0.667 0.667h-2c-0.733 0-1.333 0.6-1.333 1.333v2c0 0.373-0.293 0.667-0.667 0.667h-2.667c-0.373 0-0.667-0.293-0.667-0.667v-2c0-2.947 2.387-5.333 5.333-5.333h2c0.373 0 0.667 0.293 0.667 0.667z"></path>
<path fill="{color}" d="M17.333 24.667v-2.667c0-0.373 0.293-0.667 0.667-0.667h2c0.733 0 1.333-0.6 1.333-1.333v-2c0-0.373 0.293-0.667 0.667-0.667h2.667c0.373 0 0.667 0.293 0.667 0.667v2c0 2.947-2.387 5.333-5.333 5.333h-2c-0.373 0-0.667-0.293-0.667-0.667z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M8 11.75H5C4.59 11.75 4.25 11.41 4.25 11V9C4.25 6.38 6.38 4.25 9 4.25H11C11.41 4.25 11.75 4.59 11.75 5V8C11.75 8.41 11.41 8.75 11 8.75H9C8.86 8.75 8.75 8.86 8.75 9V11C8.75 11.41 8.41 11.75 8 11.75ZM5.75 10.25H7.25V9C7.25 8.04 8.04 7.25 9 7.25H10.25V5.75H9C7.21 5.75 5.75 7.21 5.75 9V10.25Z" fill="{color}"/>
<path d="M15 19.75H13C12.59 19.75 12.25 19.41 12.25 19V16C12.25 15.59 12.59 15.25 13 15.25H15C15.14 15.25 15.25 15.14 15.25 15V13C15.25 12.59 15.59 12.25 16 12.25H19C19.41 12.25 19.75 12.59 19.75 13V15C19.75 17.62 17.62 19.75 15 19.75ZM13.75 18.25H15C16.79 18.25 18.25 16.79 18.25 15V13.75H16.75V15C16.75 15.96 15.96 16.75 15 16.75H13.75V18.25Z" fill="{color}"/>
<path d="M15 22.75H9C3.57 22.75 1.25 20.43 1.25 15V9C1.25 3.57 3.57 1.25 9 1.25H15C20.43 1.25 22.75 3.57 22.75 9V15C22.75 20.43 20.43 22.75 15 22.75ZM9 2.75C4.39 2.75 2.75 4.39 2.75 9V15C2.75 19.61 4.39 21.25 9 21.25H15C19.61 21.25 21.25 19.61 21.25 15V9C21.25 4.39 19.61 2.75 15 2.75H9Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M11 5V8H9C8.45 8 8 8.45 8 9V11H5V9C5 6.79 6.79 5 9 5H11Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M13 19V16H15C15.55 16 16 15.55 16 15V13H19V15C19 17.21 17.21 19 15 19H13Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15 22H9C4 22 2 20 2 15V9C2 4 4 2 9 2H15C20 2 22 4 22 9V15C22 20 20 22 15 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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