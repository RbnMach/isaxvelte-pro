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
<path d="M15 22H9C4 22 2 20 2 15V9C2 4 4 2 9 2H15C20 2 22 4 22 9V15C22 20 20 22 15 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7.5 16V8H9.5C10.6 8 11.5 8.9 11.5 10C11.5 11.1 10.6 12 9.5 12H7.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16.5 11H15.2C14.5 11 14 11.6 14 12.2C14 12.9 14.6 13.4 15.2 13.4C15.9 13.4 16.4 14 16.4 14.6C16.4 15.3 15.8 15.8 15.2 15.8H14" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M9.5 8.75H8.25V11.25H9.5C10.19 11.25 10.75 10.69 10.75 10C10.75 9.31 10.19 8.75 9.5 8.75Z" fill="{color}"/>
<path d="M16.1898 2H7.81976C4.17976 2 2.00977 4.17 2.00977 7.81V16.18C2.00977 19.82 4.17976 21.99 7.81976 21.99H16.1898C19.8298 21.99 21.9998 19.82 21.9998 16.18V7.81C21.9998 4.17 19.8298 2 16.1898 2ZM9.49976 12.75H8.24976V16C8.24976 16.41 7.90976 16.75 7.49976 16.75C7.08976 16.75 6.74976 16.41 6.74976 16V8C6.74976 7.59 7.08976 7.25 7.49976 7.25H9.49976C11.0198 7.25 12.2498 8.48 12.2498 10C12.2498 11.52 11.0198 12.75 9.49976 12.75ZM15.2498 12.75C16.3498 12.75 17.2498 13.65 17.2498 14.75C17.2498 15.85 16.3498 16.75 15.2498 16.75H13.9998C13.5898 16.75 13.2498 16.41 13.2498 16C13.2498 15.59 13.5898 15.25 13.9998 15.25H15.2498C15.5298 15.25 15.7498 15.03 15.7498 14.75C15.7498 14.47 15.5298 14.25 15.2498 14.25C14.1498 14.25 13.2498 13.35 13.2498 12.25C13.2498 11.15 14.1498 10.25 15.2498 10.25H16.4998C16.9098 10.25 17.2498 10.59 17.2498 11C17.2498 11.41 16.9098 11.75 16.4998 11.75H15.2498C14.9698 11.75 14.7498 11.97 14.7498 12.25C14.7498 12.53 14.9698 12.75 15.2498 12.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M7.5 16V8H9.5C10.6 8 11.5 8.9 11.5 10C11.5 11.1 10.6 12 9.5 12H7.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16.5 11H15.25C14.56 11 14 11.56 14 12.25C14 12.94 14.56 13.5 15.25 13.5C15.94 13.5 16.5 14.06 16.5 14.75C16.5 15.44 15.94 16 15.25 16H14" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 12.83V15C2 20 4 22 9 22H15C20 22 22 20 22 15V9C22 4 20 2 15 2H9C4 2 2 4 2 9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M21.586 2.667h-11.16c-4.853 0-7.747 2.893-7.747 7.747v11.16c0 4.853 2.893 7.747 7.747 7.747h11.16c4.853 0 7.747-2.893 7.747-7.747v-11.16c0-4.853-2.893-7.747-7.747-7.747z"></path>
<path fill="{color}" d="M10 22.333c-0.547 0-1-0.453-1-1v-10.667c0-0.547 0.453-1 1-1h2.667c2.027 0 3.667 1.64 3.667 3.667s-1.64 3.667-3.667 3.667h-1.667v4.333c0 0.547-0.453 1-1 1zM11 15h1.667c0.92 0 1.667-0.747 1.667-1.667s-0.747-1.667-1.667-1.667h-1.667v3.333z"></path>
<path fill="{color}" d="M20.333 22.333h-1.667c-0.547 0-1-0.453-1-1s0.453-1 1-1h1.667c0.373 0 0.667-0.293 0.667-0.667s-0.293-0.667-0.667-0.667c-1.467 0-2.667-1.2-2.667-2.667s1.2-2.667 2.667-2.667h1.667c0.547 0 1 0.453 1 1s-0.453 1-1 1h-1.667c-0.373 0-0.667 0.293-0.667 0.667s0.293 0.667 0.667 0.667c1.467 0 2.667 1.2 2.667 2.667s-1.2 2.667-2.667 2.667z"></path>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15 22.75H9C3.57 22.75 1.25 20.43 1.25 15V9C1.25 3.57 3.57 1.25 9 1.25H15C20.43 1.25 22.75 3.57 22.75 9V15C22.75 20.43 20.43 22.75 15 22.75ZM9 2.75C4.39 2.75 2.75 4.39 2.75 9V15C2.75 19.61 4.39 21.25 9 21.25H15C19.61 21.25 21.25 19.61 21.25 15V9C21.25 4.39 19.61 2.75 15 2.75H9Z" fill="{color}"/>
<path d="M7.5 16.75C7.09 16.75 6.75 16.41 6.75 16V8C6.75 7.59 7.09 7.25 7.5 7.25H9.5C11.02 7.25 12.25 8.48 12.25 10C12.25 11.52 11.02 12.75 9.5 12.75H8.25V16C8.25 16.41 7.91 16.75 7.5 16.75ZM8.25 11.25H9.5C10.19 11.25 10.75 10.69 10.75 10C10.75 9.31 10.19 8.75 9.5 8.75H8.25V11.25Z" fill="{color}"/>
<path d="M15.25 16.75H14C13.59 16.75 13.25 16.41 13.25 16C13.25 15.59 13.59 15.25 14 15.25H15.25C15.53 15.25 15.75 15.03 15.75 14.75C15.75 14.47 15.53 14.25 15.25 14.25C14.15 14.25 13.25 13.35 13.25 12.25C13.25 11.15 14.15 10.25 15.25 10.25H16.5C16.91 10.25 17.25 10.59 17.25 11C17.25 11.41 16.91 11.75 16.5 11.75H15.25C14.97 11.75 14.75 11.97 14.75 12.25C14.75 12.53 14.97 12.75 15.25 12.75C16.35 12.75 17.25 13.65 17.25 14.75C17.25 15.85 16.35 16.75 15.25 16.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15 22H9C4 22 2 20 2 15V9C2 4 4 2 9 2H15C20 2 22 4 22 9V15C22 20 20 22 15 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M7.5 16V8H9.5C10.6 8 11.5 8.9 11.5 10C11.5 11.1 10.6 12 9.5 12H7.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M16.5 11H15.25C14.56 11 14 11.56 14 12.25C14 12.94 14.56 13.5 15.25 13.5C15.94 13.5 16.5 14.06 16.5 14.75C16.5 15.44 15.94 16 15.25 16H14" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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