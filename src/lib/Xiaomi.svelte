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
<path d="M7.5 15V9H11.5C12.6 9 13.5 9.9 13.5 11V15" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10.5 15V12" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16.5 15V9" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM11.25 15C11.25 15.41 10.91 15.75 10.5 15.75C10.09 15.75 9.75 15.41 9.75 15V12C9.75 11.59 10.09 11.25 10.5 11.25C10.91 11.25 11.25 11.59 11.25 12V15ZM14.25 15C14.25 15.41 13.91 15.75 13.5 15.75C13.09 15.75 12.75 15.41 12.75 15V11C12.75 10.31 12.19 9.75 11.5 9.75H8.25V15C8.25 15.41 7.91 15.75 7.5 15.75C7.09 15.75 6.75 15.41 6.75 15V9C6.75 8.59 7.09 8.25 7.5 8.25H11.5C13.02 8.25 14.25 9.48 14.25 11V15ZM17.25 15C17.25 15.41 16.91 15.75 16.5 15.75C16.09 15.75 15.75 15.41 15.75 15V9C15.75 8.59 16.09 8.25 16.5 8.25C16.91 8.25 17.25 8.59 17.25 9V15Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M7.5 15V9H11.5C12.6 9 13.5 9.9 13.5 11V15" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10.5 15V12" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16.5 15V9" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.19997 2.30001 7.96997 2.85001" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M18 21c-0.547 0-1-0.453-1-1v-5.333c0-0.92-0.747-1.667-1.667-1.667h-4.333v7c0 0.547-0.453 1-1 1s-1-0.453-1-1v-8c0-0.547 0.453-1 1-1h5.333c2.027 0 3.667 1.64 3.667 3.667v5.333c0 0.547-0.453 1-1 1z"></path>
<path fill="{color}" d="M14 21c-0.547 0-1-0.453-1-1v-4c0-0.547 0.453-1 1-1s1 0.453 1 1v4c0 0.547-0.453 1-1 1z"></path>
<path fill="{color}" d="M22 21c-0.547 0-1-0.453-1-1v-8c0-0.547 0.453-1 1-1s1 0.453 1 1v8c0 0.547-0.453 1-1 1z"></path>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M13.5 15.75C13.09 15.75 12.75 15.41 12.75 15V11C12.75 10.31 12.19 9.75 11.5 9.75H8.25V15C8.25 15.41 7.91 15.75 7.5 15.75C7.09 15.75 6.75 15.41 6.75 15V9C6.75 8.59 7.09 8.25 7.5 8.25H11.5C13.02 8.25 14.25 9.48 14.25 11V15C14.25 15.41 13.91 15.75 13.5 15.75Z" fill="{color}"/>
<path d="M10.5 15.75C10.09 15.75 9.75 15.41 9.75 15V12C9.75 11.59 10.09 11.25 10.5 11.25C10.91 11.25 11.25 11.59 11.25 12V15C11.25 15.41 10.91 15.75 10.5 15.75Z" fill="{color}"/>
<path d="M16.5 15.75C16.09 15.75 15.75 15.41 15.75 15V9C15.75 8.59 16.09 8.25 16.5 8.25C16.91 8.25 17.25 8.59 17.25 9V15C17.25 15.41 16.91 15.75 16.5 15.75Z" fill="{color}"/>
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M7.5 15V9H11.5C12.6 9 13.5 9.9 13.5 11V15" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M10.5 15V12" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M16.5 15V9" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
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