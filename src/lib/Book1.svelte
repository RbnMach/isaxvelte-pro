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
<path d="M3.5 18V7C3.5 3 4.5 2 8.5 2H15.5C19.5 2 20.5 3 20.5 7V17C20.5 17.14 20.5 17.28 20.49 17.42" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6.35 15H20.5V18.5C20.5 20.43 18.93 22 17 22H7C5.07 22 3.5 20.43 3.5 18.5V17.85C3.5 16.28 4.78 15 6.35 15Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8 7H16" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8 10.5H13" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M20.5 16V18.5C20.5 20.43 18.93 22 17 22H7C5.07 22 3.5 20.43 3.5 18.5V17.85C3.5 16.28 4.78 15 6.35 15H19.5C20.05 15 20.5 15.45 20.5 16Z" fill="{color}"/>
<path d="M15.5 2H8.5C4.5 2 3.5 3 3.5 7V14.58C4.26 13.91 5.26 13.5 6.35 13.5H19.5C20.05 13.5 20.5 13.05 20.5 12.5V7C20.5 3 19.5 2 15.5 2ZM13 10.75H8C7.59 10.75 7.25 10.41 7.25 10C7.25 9.59 7.59 9.25 8 9.25H13C13.41 9.25 13.75 9.59 13.75 10C13.75 10.41 13.41 10.75 13 10.75ZM16 7.25H8C7.59 7.25 7.25 6.91 7.25 6.5C7.25 6.09 7.59 5.75 8 5.75H16C16.41 5.75 16.75 6.09 16.75 6.5C16.75 6.91 16.41 7.25 16 7.25Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M20.5002 11V17C20.5002 17.14 20.5002 17.28 20.4902 17.42" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3.5 18V7C3.5 3 4.5 2 8.5 2H15.5C19.5 2 20.5 3 20.5 7" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6.35 15H20.5V18.5C20.5 20.43 18.93 22 17 22H7C5.07 22 3.5 20.43 3.5 18.5V17.85C3.5 16.28 4.78 15 6.35 15Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8 7H16" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8 10.5H13" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M20.5 7V15H6.35C4.78 15 3.5 16.28 3.5 17.85V7C3.5 3 4.5 2 8.5 2H15.5C19.5 2 20.5 3 20.5 7Z" fill="{color}"/>
<path d="M20.5 15V18.5C20.5 20.43 18.93 22 17 22H7C5.07 22 3.5 20.43 3.5 18.5V17.85C3.5 16.28 4.78 15 6.35 15H20.5Z" fill="{color}"/>
<path d="M16 7.75H8C7.59 7.75 7.25 7.41 7.25 7C7.25 6.59 7.59 6.25 8 6.25H16C16.41 6.25 16.75 6.59 16.75 7C16.75 7.41 16.41 7.75 16 7.75Z" fill="{color}"/>
<path d="M13 11.25H8C7.59 11.25 7.25 10.91 7.25 10.5C7.25 10.09 7.59 9.75 8 9.75H13C13.41 9.75 13.75 10.09 13.75 10.5C13.75 10.91 13.41 11.25 13 11.25Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M3.5 18.75C3.09 18.75 2.75 18.41 2.75 18V7C2.75 2.59 4.09 1.25 8.5 1.25H15.5C19.91 1.25 21.25 2.59 21.25 7V17C21.25 17.16 21.25 17.31 21.24 17.47C21.21 17.88 20.84 18.2 20.44 18.17C20.03 18.14 19.71 17.78 19.74 17.37C19.75 17.25 19.75 17.12 19.75 17V7C19.75 3.43 19.08 2.75 15.5 2.75H8.5C4.92 2.75 4.25 3.43 4.25 7V18C4.25 18.41 3.91 18.75 3.5 18.75Z" fill="{color}"/>
<path d="M17 22.75H7C4.66 22.75 2.75 20.84 2.75 18.5V17.85C2.75 15.86 4.37 14.25 6.35 14.25H20.5C20.91 14.25 21.25 14.59 21.25 15V18.5C21.25 20.84 19.34 22.75 17 22.75ZM6.35 15.75C5.19 15.75 4.25 16.69 4.25 17.85V18.5C4.25 20.02 5.48 21.25 7 21.25H17C18.52 21.25 19.75 20.02 19.75 18.5V15.75H6.35Z" fill="{color}"/>
<path d="M16 7.75H8C7.59 7.75 7.25 7.41 7.25 7C7.25 6.59 7.59 6.25 8 6.25H16C16.41 6.25 16.75 6.59 16.75 7C16.75 7.41 16.41 7.75 16 7.75Z" fill="{color}"/>
<path d="M13 11.25H8C7.59 11.25 7.25 10.91 7.25 10.5C7.25 10.09 7.59 9.75 8 9.75H13C13.41 9.75 13.75 10.09 13.75 10.5C13.75 10.91 13.41 11.25 13 11.25Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M3.5 18V7C3.5 3 4.5 2 8.5 2H15.5C19.5 2 20.5 3 20.5 7V17C20.5 17.14 20.5 17.28 20.49 17.42" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6.35 15H20.5V18.5C20.5 20.43 18.93 22 17 22H7C5.07 22 3.5 20.43 3.5 18.5V17.85C3.5 16.28 4.78 15 6.35 15Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M8 7H16" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M8 10.5H13" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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