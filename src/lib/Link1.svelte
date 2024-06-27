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
<path d="M14.99 17.5H16.5C19.52 17.5 22 15.03 22 12C22 8.98 19.53 6.5 16.5 6.5H14.99" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9 6.5H7.5C4.47 6.5 2 8.97 2 12C2 15.02 4.47 17.5 7.5 17.5H9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8 12H16" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M7.24989 12C7.24989 11.59 7.58989 11.25 7.99989 11.25H10.9999V7.5C10.9999 6.95 10.5499 6.5 9.99989 6.5H7.76989C4.61989 6.5 1.87989 9.08 1.99989 12.22C2.05989 13.65 2.65989 14.94 3.60989 15.89C4.60989 16.88 5.97989 17.5 7.49989 17.5H9.99989C10.5499 17.5 10.9999 17.05 10.9999 16.5V12.75H7.99989C7.58989 12.75 7.24989 12.41 7.24989 12Z" fill="{color}"/>
<path d="M20.39 8.11C19.39 7.12 18.02 6.5 16.5 6.5H14C13.45 6.5 13 6.95 13 7.5V11.25H16C16.41 11.25 16.75 11.59 16.75 12C16.75 12.41 16.41 12.75 16 12.75H13V16.5C13 17.05 13.45 17.5 14 17.5H16.23C19.38 17.5 22.12 14.92 21.99 11.78C21.94 10.35 21.33 9.06 20.39 8.11Z" fill="{color}"/>
<path d="M13 11.25H11V12.75H13V11.25Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M14.9902 17.5H16.5002C19.5202 17.5 22.0002 15.03 22.0002 12C22.0002 8.98 19.5302 6.5 16.5002 6.5H14.9902" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2.37 10.01C2.13 10.63 2 11.3 2 12C2 15.02 4.47 17.5 7.5 17.5H9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.99969 6.5H7.49969C6.66969 6.5 5.88969 6.68 5.17969 7.01" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8 12H16" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M10.9999 7.5V16.5C10.9999 17.05 10.5499 17.5 9.99989 17.5H7.49989C5.97989 17.5 4.60989 16.88 3.60989 15.89C2.66989 14.94 2.05989 13.65 1.99989 12.22C1.87989 9.08 4.61989 6.5 7.76989 6.5H9.99989C10.5499 6.5 10.9999 6.95 10.9999 7.5Z" fill="{color}"/>
<path opacity="0.4" d="M21.9998 11.78C22.1298 14.93 19.3898 17.5 16.2398 17.5H14.0098C13.4598 17.5 13.0098 17.05 13.0098 16.5V7.5C13.0098 6.95 13.4598 6.5 14.0098 6.5H16.5098C18.0298 6.5 19.3998 7.12 20.3998 8.11C21.3298 9.06 21.9398 10.35 21.9998 11.78Z" fill="{color}"/>
<path d="M16 12.75H8C7.59 12.75 7.25 12.41 7.25 12C7.25 11.59 7.59 11.25 8 11.25H16C16.41 11.25 16.75 11.59 16.75 12C16.75 12.41 16.41 12.75 16 12.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.5002 18.25H14.9902C14.5802 18.25 14.2402 17.91 14.2402 17.5C14.2402 17.09 14.5802 16.75 14.9902 16.75H16.5002C19.1202 16.75 21.2502 14.62 21.2502 12C21.2502 9.38 19.1202 7.25 16.5002 7.25H15.0002C14.5902 7.25 14.2502 6.91 14.2502 6.5C14.2502 6.09 14.5802 5.75 15.0002 5.75H16.5002C19.9502 5.75 22.7502 8.55 22.7502 12C22.7502 15.45 19.9502 18.25 16.5002 18.25Z" fill="{color}"/>
<path d="M9 18.25H7.5C4.05 18.25 1.25 15.45 1.25 12C1.25 8.55 4.05 5.75 7.5 5.75H9C9.41 5.75 9.75 6.09 9.75 6.5C9.75 6.91 9.41 7.25 9 7.25H7.5C4.88 7.25 2.75 9.38 2.75 12C2.75 14.62 4.88 16.75 7.5 16.75H9C9.41 16.75 9.75 17.09 9.75 17.5C9.75 17.91 9.41 18.25 9 18.25Z" fill="{color}"/>
<path d="M16 12.75H8C7.59 12.75 7.25 12.41 7.25 12C7.25 11.59 7.59 11.25 8 11.25H16C16.41 11.25 16.75 11.59 16.75 12C16.75 12.41 16.41 12.75 16 12.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M14.9902 17.5H16.5002C19.5202 17.5 22.0002 15.03 22.0002 12C22.0002 8.98 19.5302 6.5 16.5002 6.5H14.9902" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9 6.5H7.5C4.47 6.5 2 8.97 2 12C2 15.02 4.47 17.5 7.5 17.5H9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M8 12H16" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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