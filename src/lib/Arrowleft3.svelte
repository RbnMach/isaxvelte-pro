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
<path d="M17.9999 12.0001V14.6701C17.9999 17.9801 15.6499 19.3401 12.7799 17.6801L10.4699 16.3401L8.15995 15.0001C5.28995 13.3401 5.28995 10.6301 8.15995 8.97005L10.4699 7.63005L12.7799 6.29005C15.6499 4.66005 17.9999 6.01005 17.9999 9.33005V12.0001Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M18 9.32919V14.6692C18 17.9892 15.65 19.3392 12.78 17.6892L11.5 16.9492C11.19 16.7692 11 16.4392 11 16.0792V7.91919C11 7.55919 11.19 7.22919 11.5 7.04919L12.78 6.30919C15.65 4.65919 18 6.00919 18 9.32919Z" fill="{color}"/>
<path d="M9.99859 8.79152V15.2215C9.99859 15.6115 9.57859 15.8515 9.24859 15.6515L8.14859 15.0115C5.27859 13.3615 5.27859 10.6415 8.14859 8.99152L9.24859 8.35152C9.57859 8.16152 9.99859 8.40152 9.99859 8.79152Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12.7803 6.30992C15.6503 4.65992 18.0003 6.00993 18.0003 9.32993V11.9999V14.6699C18.0003 17.9799 15.6503 19.3399 12.7803 17.6799L10.4703 16.3399L8.16031 14.9999C5.29031 13.3399 5.29031 10.6299 8.16031 8.96993" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M18 9.32993V14.6699C18 17.9899 15.65 19.3399 12.78 17.6899L11.5 16.9499C11.19 16.7699 11 16.4399 11 16.0799V7.91993C11 7.55993 11.19 7.22993 11.5 7.04993L12.78 6.30992C15.65 4.65992 18 6.00993 18 9.32993Z" fill="{color}"/>
<path opacity="0.4" d="M10.0005 8.79006V15.2201C10.0005 15.6101 9.58055 15.8501 9.25055 15.6501L8.15055 15.0101C5.28055 13.3601 5.28055 10.6401 8.15055 8.99006L9.25055 8.35006C9.58055 8.16006 10.0005 8.40006 10.0005 8.79006Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15.1 19.1498C14.26 19.1498 13.34 18.8798 12.41 18.3398L7.78 15.6698C6.15 14.7198 5.25 13.4198 5.25 11.9998C5.25 10.5798 6.15 9.2798 7.78 8.3398L12.41 5.6698C14.04 4.7298 15.61 4.5998 16.85 5.3098C18.08 6.0198 18.76 7.4498 18.76 9.3298V14.6698C18.76 16.5498 18.08 17.9798 16.85 18.6898C16.32 18.9998 15.73 19.1498 15.1 19.1498ZM15.1 6.3598C14.52 6.3598 13.86 6.5598 13.16 6.9698L8.53 9.6398C7.38 10.2998 6.75 11.1398 6.75 11.9998C6.75 12.8598 7.38 13.6998 8.53 14.3598L13.16 17.0298C14.31 17.6898 15.35 17.8198 16.1 17.3898C16.85 16.9598 17.26 15.9898 17.26 14.6698V9.3298C17.26 8.0098 16.85 7.0398 16.1 6.6098C15.8 6.4398 15.46 6.3598 15.1 6.3598Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M18.0003 12.0001V14.6701C18.0003 17.9801 15.6503 19.3401 12.7803 17.6801L10.4703 16.3401L8.16031 15.0001C5.29031 13.3401 5.29031 10.6301 8.16031 8.97005L10.4703 7.63005L12.7803 6.29005C15.6503 4.66005 18.0003 6.01005 18.0003 9.33005V12.0001Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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