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
<path d="M9 22H15C20 22 22 20 22 15V9C22 4 20 2 15 2H9C4 2 2 4 2 9V15C2 20 4 22 9 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.5 18.5C16.6 18.5 17.5 17.6 17.5 16.5V7.5C17.5 6.4 16.6 5.5 15.5 5.5C14.4 5.5 13.5 6.4 13.5 7.5V16.5C13.5 17.6 14.39 18.5 15.5 18.5Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.5 18.5C9.6 18.5 10.5 17.6 10.5 16.5V13C10.5 11.9 9.6 11 8.5 11C7.4 11 6.5 11.9 6.5 13V16.5C6.5 17.6 7.39 18.5 8.5 18.5Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.19 2H7.81C4.17 2 2 4.17 2 7.81V16.18C2 19.83 4.17 22 7.81 22H16.18C19.82 22 21.99 19.83 21.99 16.19V7.81C22 4.17 19.83 2 16.19 2ZM9.91 16.19C9.91 16.83 9.39 17.35 8.74 17.35C8.1 17.35 7.58 16.83 7.58 16.19V12.93C7.58 12.29 8.1 11.77 8.74 11.77C9.39 11.77 9.91 12.29 9.91 12.93V16.19ZM16.42 16.19C16.42 16.83 15.9 17.35 15.26 17.35C14.61 17.35 14.09 16.83 14.09 16.19V7.81C14.09 7.17 14.61 6.65 15.26 6.65C15.9 6.65 16.42 7.17 16.42 7.81V16.19Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2 13.01V15C2 20 4 22 9 22H15C20 22 22 20 22 15V9C22 4 20 2 15 2H9C4 2 2 4 2 9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17.5 11.57V16.5C17.5 17.6 16.61 18.5 15.5 18.5C14.4 18.5 13.5 17.6 13.5 16.5V7.5C13.5 6.4 14.4 5.5 15.5 5.5C16.6 5.5 17.5 6.4 17.5 7.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.5 18.5C9.6 18.5 10.5 17.6 10.5 16.5V13C10.5 11.9 9.6 11 8.5 11C7.4 11 6.5 11.9 6.5 13V16.5C6.5 17.6 7.39 18.5 8.5 18.5Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M16.19 2H7.81C4.17 2 2 4.17 2 7.81V16.18C2 19.83 4.17 22 7.81 22H16.18C19.82 22 21.99 19.83 21.99 16.19V7.81C22 4.17 19.83 2 16.19 2Z" fill="{color}"/>
<path d="M16.4198 7.8099V16.1899C16.4198 16.8299 15.8998 17.3499 15.2598 17.3499C14.6098 17.3499 14.0898 16.8299 14.0898 16.1899V7.8099C14.0898 7.1699 14.6098 6.6499 15.2598 6.6499C15.8998 6.6499 16.4198 7.1699 16.4198 7.8099Z" fill="{color}"/>
<path d="M9.91008 12.93V16.19C9.91008 16.83 9.39008 17.35 8.74008 17.35C8.10008 17.35 7.58008 16.83 7.58008 16.19V12.93C7.58008 12.29 8.10008 11.77 8.74008 11.77C9.39008 11.77 9.91008 12.29 9.91008 12.93Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15 22.75H9C3.57 22.75 1.25 20.43 1.25 15V9C1.25 3.57 3.57 1.25 9 1.25H15C20.43 1.25 22.75 3.57 22.75 9V15C22.75 20.43 20.43 22.75 15 22.75ZM9 2.75C4.39 2.75 2.75 4.39 2.75 9V15C2.75 19.61 4.39 21.25 9 21.25H15C19.61 21.25 21.25 19.61 21.25 15V9C21.25 4.39 19.61 2.75 15 2.75H9Z" fill="{color}"/>
<path d="M15.5 19.25C13.98 19.25 12.75 18.02 12.75 16.5V7.5C12.75 5.98 13.98 4.75 15.5 4.75C17.02 4.75 18.25 5.98 18.25 7.5V16.5C18.25 18.02 17.02 19.25 15.5 19.25ZM15.5 6.25C14.81 6.25 14.25 6.81 14.25 7.5V16.5C14.25 17.19 14.81 17.75 15.5 17.75C16.19 17.75 16.75 17.19 16.75 16.5V7.5C16.75 6.81 16.19 6.25 15.5 6.25Z" fill="{color}"/>
<path d="M8.5 19.25C6.98 19.25 5.75 18.02 5.75 16.5V13C5.75 11.48 6.98 10.25 8.5 10.25C10.02 10.25 11.25 11.48 11.25 13V16.5C11.25 18.02 10.02 19.25 8.5 19.25ZM8.5 11.75C7.81 11.75 7.25 12.31 7.25 13V16.5C7.25 17.19 7.81 17.75 8.5 17.75C9.19 17.75 9.75 17.19 9.75 16.5V13C9.75 12.31 9.19 11.75 8.5 11.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M9 22H15C20 22 22 20 22 15V9C22 4 20 2 15 2H9C4 2 2 4 2 9V15C2 20 4 22 9 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M15.5 18.5C16.6 18.5 17.5 17.6 17.5 16.5V7.5C17.5 6.4 16.6 5.5 15.5 5.5C14.4 5.5 13.5 6.4 13.5 7.5V16.5C13.5 17.6 14.39 18.5 15.5 18.5Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M8.5 18.5C9.6 18.5 10.5 17.6 10.5 16.5V13C10.5 11.9 9.6 11 8.5 11C7.4 11 6.5 11.9 6.5 13V16.5C6.5 17.6 7.39 18.5 8.5 18.5Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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