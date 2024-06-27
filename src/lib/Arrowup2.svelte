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
<path d="M12 18.0001H9.33004C6.02005 18.0001 4.66005 15.6501 6.32005 12.7801L7.66004 10.4701L9.00005 8.16007C10.66 5.29007 13.37 5.29007 15.03 8.16007L16.37 10.4701L17.71 12.7801C19.37 15.6501 18.01 18.0001 14.7 18.0001H12Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M9.32919 18H14.6692C17.9892 18 19.3392 15.65 17.6892 12.78L16.9492 11.5C16.7692 11.19 16.4392 11 16.0792 11H7.91919C7.55919 11 7.22919 11.19 7.04919 11.5L6.30919 12.78C4.65919 15.65 6.00919 18 9.32919 18Z" fill="{color}"/>
<path d="M8.79152 9.99859H15.2215C15.6115 9.99859 15.8515 9.57859 15.6515 9.24859L15.0115 8.14859C13.3615 5.27859 10.6415 5.27859 8.99152 8.14859L8.35152 9.24859C8.16152 9.57859 8.40152 9.99859 8.79152 9.99859Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M17.6897 12.7801C19.3497 15.6501 17.9897 18.0001 14.6797 18.0001H11.9997H9.32968C6.01968 18.0001 4.65968 15.6501 6.31968 12.7801L7.65968 10.4701L8.99968 8.16007C10.6597 5.29007 13.3697 5.29007 15.0297 8.16007" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M9.32919 18H14.6692C17.9892 18 19.3392 15.65 17.6892 12.78L16.9492 11.5C16.7692 11.19 16.4392 11 16.0792 11H7.91919C7.55919 11 7.22919 11.19 7.04919 11.5L6.30919 12.78C4.65919 15.65 6.00919 18 9.32919 18Z" fill="{color}"/>
<path opacity="0.4" d="M8.78957 10.0001H15.2196C15.6096 10.0001 15.8496 9.58006 15.6496 9.25006L15.0096 8.15006C13.3596 5.28006 10.6396 5.28006 8.98957 8.15006L8.34957 9.25006C8.15957 9.58006 8.39957 10.0001 8.78957 10.0001Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M14.6698 18.75H9.3298C7.4498 18.75 6.0198 18.07 5.3098 16.84C4.5998 15.61 4.7298 14.03 5.6698 12.4L8.3398 7.77C9.2798 6.15 10.5798 5.25 11.9998 5.25C13.4198 5.25 14.7198 6.15 15.6598 7.78L18.3298 12.41C19.2698 14.04 19.3998 15.62 18.6898 16.85C17.9798 18.07 16.5498 18.75 14.6698 18.75ZM11.9998 6.75C11.1398 6.75 10.2998 7.38 9.6398 8.53L6.9698 13.16C6.3098 14.31 6.1798 15.35 6.6098 16.1C7.0398 16.85 8.0098 17.26 9.3298 17.26H14.6698C15.9898 17.26 16.9598 16.85 17.3898 16.1C17.8198 15.35 17.6898 14.31 17.0298 13.16L14.3598 8.53C13.6998 7.38 12.8598 6.75 11.9998 6.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11.9997 17.9998H9.32968C6.01968 17.9998 4.65968 15.6498 6.31968 12.7798L7.65968 10.4698L8.99968 8.15982C10.6597 5.28982 13.3697 5.28982 15.0297 8.15982L16.3697 10.4698L17.7097 12.7798C19.3697 15.6498 18.0097 17.9998 14.6997 17.9998H11.9997Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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