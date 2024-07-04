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
<path d="M6 11.9999V9.32992C6 6.01992 8.35 4.65992 11.22 6.31992L13.53 7.65992L15.84 8.99992C18.71 10.6599 18.71 13.3699 15.84 15.0299L13.53 16.3699L11.22 17.7099C8.35 19.3399 6 17.9899 6 14.6699V11.9999Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M6 9.32919V14.6692C6 17.9892 8.35 19.3392 11.22 17.6892L12.5 16.9492C12.81 16.7692 13 16.4392 13 16.0792V7.91919C13 7.55919 12.81 7.22919 12.5 7.04919L11.22 6.30919C8.35 4.65919 6 6.00919 6 9.32919Z" fill="{color}"/>
<path d="M14 8.79152V15.2215C14 15.6115 14.42 15.8515 14.75 15.6515L15.85 15.0115C18.72 13.3615 18.72 10.6415 15.85 8.99152L14.75 8.35152C14.42 8.16152 14 8.40152 14 8.79152Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15.85 8.98992C18.72 10.6499 18.72 13.3599 15.85 15.0199L13.54 16.3599L11.23 17.6999C8.35 19.3399 6 17.9899 6 14.6699V11.9999V9.32992C6 6.01992 8.35 4.65992 11.22 6.31992" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M6 9.32993V14.6699C6 17.9899 8.35 19.3399 11.22 17.6899L12.5 16.9499C12.81 16.7699 13 16.4399 13 16.0799V7.91993C13 7.55993 12.81 7.22993 12.5 7.04993L11.22 6.30992C8.35 4.65992 6 6.00993 6 9.32993Z" fill="{color}"/>
<path opacity="0.4" d="M14 8.79006V15.2201C14 15.6101 14.42 15.8501 14.75 15.6501L15.85 15.0101C18.72 13.3601 18.72 10.6401 15.85 8.99006L14.75 8.35006C14.42 8.16006 14 8.40006 14 8.79006Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M8.9 19.1498C8.27 19.1498 7.68 18.9998 7.16 18.6998C5.93 17.9898 5.25 16.5598 5.25 14.6798V9.3298C5.25 7.4498 5.93 6.0198 7.16 5.3098C8.39 4.5998 9.96 4.7298 11.6 5.6698L16.23 8.3398C17.86 9.2798 18.76 10.5798 18.76 11.9998C18.76 13.4198 17.86 14.7198 16.23 15.6598L11.6 18.3298C10.66 18.8798 9.74 19.1498 8.9 19.1498ZM8.9 6.3598C8.53 6.3598 8.19 6.4398 7.9 6.6098C7.16 7.0398 6.75 7.9998 6.75 9.3298V14.6698C6.75 15.9898 7.16 16.9598 7.91 17.3898C8.66 17.8198 9.7 17.6898 10.85 17.0298L15.48 14.3598C16.63 13.6998 17.26 12.8598 17.26 11.9998C17.26 11.1398 16.63 10.2998 15.48 9.6398L10.85 6.9698C10.14 6.5598 9.48 6.3598 8.9 6.3598Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M6 12.0002V9.33017C6 6.02017 8.35 4.66017 11.22 6.32017L13.53 7.66017L15.84 9.00017C18.71 10.6602 18.71 13.3702 15.84 15.0302L13.53 16.3702L11.22 17.7102C8.35 19.3402 6 17.9902 6 14.6702V12.0002Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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