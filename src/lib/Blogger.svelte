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
<path d="M6 9V15C6 17 7 18 9 18H15C17 18 18 17 18 15V12C18 11.4 17.6 11 17 11C16.4 11 16 10.6 16 10V9C16 7 15 6 13 6H9C7 6 6 7 6 9Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path d="M10 10H12" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10 14H14" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15 22H9C4 22 2 20 2 15V9C2 4 4 2 9 2H15C20 2 22 4 22 9V15C22 20 20 22 15 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M14 13.25H10C9.59 13.25 9.25 13.59 9.25 14C9.25 14.41 9.59 14.75 10 14.75H14C14.41 14.75 14.75 14.41 14.75 14C14.75 13.59 14.41 13.25 14 13.25Z" fill="{color}"/>
<path d="M10 10.75H12C12.41 10.75 12.75 10.41 12.75 10C12.75 9.59 12.41 9.25 12 9.25H10C9.59 9.25 9.25 9.59 9.25 10C9.25 10.41 9.59 10.75 10 10.75Z" fill="{color}"/>
<path d="M16.1898 2H7.81976C4.17976 2 2.00977 4.17 2.00977 7.81V16.18C2.00977 19.82 4.17976 21.99 7.81976 21.99H16.1898C19.8298 21.99 21.9998 19.82 21.9998 16.18V7.81C21.9998 4.17 19.8298 2 16.1898 2ZM17.9998 15C17.9998 17 16.9998 18 14.9998 18H8.99976C6.99976 18 5.99976 17 5.99976 15V9C5.99976 7 6.99976 6 8.99976 6H12.9998C14.9998 6 15.9998 7 15.9998 9V10C15.9998 10.55 16.4498 11 16.9998 11C17.5498 11 17.9998 11.45 17.9998 12V15Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M6 9V15C6 17 7 18 9 18H15C17 18 18 17 18 15V12C18 11.45 17.55 11 17 11C16.45 11 16 10.55 16 10V9C16 7 15 6 13 6H9C7 6 6 7 6 9Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path d="M10 10H12" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10 14H14" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 12.83V15C2 20 4 22 9 22H15C20 22 22 20 22 15V9C22 4 20 2 15 2H9C4 2 2 4 2 9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" d="M22.667 14.667c-0.733 0-1.333-0.6-1.333-1.333v-1.333c0-2.667-1.333-4-4-4h-5.333c-2.667 0-4 1.333-4 4v8c0 2.667 1.333 4 4 4h8c2.667 0 4-1.333 4-4v-4c0-0.733-0.6-1.333-1.333-1.333zM13.333 12.333h2.667c0.547 0 1 0.453 1 1s-0.453 1-1 1h-2.667c-0.547 0-1-0.453-1-1s0.453-1 1-1zM18.667 19.667h-5.333c-0.547 0-1-0.453-1-1s0.453-1 1-1h5.333c0.547 0 1 0.453 1 1s-0.453 1-1 1z"></path>
<path fill="{color}" opacity="0.4" d="M21.586 2.667h-11.16c-4.853 0-7.747 2.893-7.747 7.747v11.16c0 4.853 2.893 7.747 7.747 7.747h11.16c4.853 0 7.747-2.893 7.747-7.747v-11.16c0-4.853-2.893-7.747-7.747-7.747z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15 18.75H9C6.58 18.75 5.25 17.42 5.25 15V9C5.25 6.58 6.58 5.25 9 5.25H13C15.42 5.25 16.75 6.58 16.75 9V10C16.75 10.14 16.86 10.25 17 10.25C17.96 10.25 18.75 11.04 18.75 12V15C18.75 17.42 17.42 18.75 15 18.75ZM9 6.75C7.42 6.75 6.75 7.42 6.75 9V15C6.75 16.58 7.42 17.25 9 17.25H15C16.58 17.25 17.25 16.58 17.25 15V12C17.25 11.86 17.14 11.75 17 11.75C16.04 11.75 15.25 10.96 15.25 10V9C15.25 7.42 14.58 6.75 13 6.75H9Z" fill="{color}"/>
<path d="M12 10.75H10C9.59 10.75 9.25 10.41 9.25 10C9.25 9.59 9.59 9.25 10 9.25H12C12.41 9.25 12.75 9.59 12.75 10C12.75 10.41 12.41 10.75 12 10.75Z" fill="{color}"/>
<path d="M14 14.75H10C9.59 14.75 9.25 14.41 9.25 14C9.25 13.59 9.59 13.25 10 13.25H14C14.41 13.25 14.75 13.59 14.75 14C14.75 14.41 14.41 14.75 14 14.75Z" fill="{color}"/>
<path d="M15 22.75H9C3.57 22.75 1.25 20.43 1.25 15V9C1.25 3.57 3.57 1.25 9 1.25H15C20.43 1.25 22.75 3.57 22.75 9V15C22.75 20.43 20.43 22.75 15 22.75ZM9 2.75C4.39 2.75 2.75 4.39 2.75 9V15C2.75 19.61 4.39 21.25 9 21.25H15C19.61 21.25 21.25 19.61 21.25 15V9C21.25 4.39 19.61 2.75 15 2.75H9Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M6 9V15C6 17 7 18 9 18H15C17 18 18 17 18 15V12C18 11.45 17.55 11 17 11C16.45 11 16 10.55 16 10V9C16 7 15 6 13 6H9C7 6 6 7 6 9Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path opacity="0.4" d="M10 10H12" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M10 14H14" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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