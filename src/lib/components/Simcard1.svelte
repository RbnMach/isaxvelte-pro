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
<path d="M19.54 6.54L16.47 3.47C15.53 2.53 14.26 2 12.93 2H8C5 2 3 4 3 7V17C3 20 5 22 8 22H16C19 22 21 20 21 17V10.07C21 8.74 20.47 7.47 19.54 6.54Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10 18.5H14C15.65 18.5 17 17.15 17 15.5V12.5C17 10.85 15.65 9.5 14 9.5H10C8.35 9.5 7 10.85 7 12.5V15.5C7 17.15 8.35 18.5 10 18.5Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 9.5V18.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7.5 14H16.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M19.54 6.54L16.47 3.47C15.53 2.53 14.26 2 12.93 2H8C5 2 3 4 3 7V17C3 20 5 22 8 22H16C19 22 21 20 21 17V10.07C21 8.74 20.47 7.47 19.54 6.54ZM11.5 18C11.5 18.2761 11.2761 18.5 11 18.5H10C8.35 18.5 7 17.15 7 15.5V15C7 14.7239 7.22386 14.5 7.5 14.5H11.25C11.39 14.5 11.5 14.61 11.5 14.75V18ZM11.5 13.25C11.5 13.39 11.39 13.5 11.25 13.5H7.5C7.22386 13.5 7 13.2761 7 13V12.5C7 10.85 8.35 9.5 10 9.5H11C11.2761 9.5 11.5 9.72386 11.5 10V13.25ZM17 15.5C17 17.15 15.65 18.5 14 18.5H13C12.7239 18.5 12.5 18.2761 12.5 18V14.75C12.5 14.61 12.61 14.5 12.75 14.5H16.5C16.7761 14.5 17 14.7239 17 15V15.5ZM17 13C17 13.2761 16.7761 13.5 16.5 13.5H12.75C12.61 13.5 12.5 13.39 12.5 13.25V10C12.5 9.72386 12.7239 9.5 13 9.5H14C15.65 9.5 17 10.85 17 12.5V13Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M3 17C3 20 5 22 8 22H16C19 22 21 20 21 17V10.07C21 8.74 20.47 7.47 19.54 6.53L16.47 3.46C15.53 2.53 14.26 2 12.93 2H8C5 2 3 4 3 7V12.98" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10 18.5H14C15.65 18.5 17 17.15 17 15.5V12.5C17 10.85 15.65 9.5 14 9.5H10C8.35 9.5 7 10.85 7 12.5V15.5C7 17.15 8.35 18.5 10 18.5Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 9.5V18.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7.5 14H16.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M19.54 6.54L16.47 3.47C15.53 2.53 14.26 2 12.93 2H8C5 2 3 4 3 7V17C3 20 5 22 8 22H16C19 22 21 20 21 17V10.07C21 8.74 20.47 7.47 19.54 6.54Z" fill="{color}"/>
<path d="M11.5 13.25V9.5H10C8.35 9.5 7 10.85 7 12.5V13.5H11.25C11.39 13.5 11.5 13.39 11.5 13.25Z" fill="{color}"/>
<path d="M12.75 13.5H17V12.5C17 10.85 15.65 9.5 14 9.5H12.5V13.25C12.5 13.39 12.61 13.5 12.75 13.5Z" fill="{color}"/>
<path d="M11.25 14.5H7V15.5C7 17.15 8.35 18.5 10 18.5H11.5V14.75C11.5 14.61 11.39 14.5 11.25 14.5Z" fill="{color}"/>
<path d="M12.5 14.75V18.5H14C15.65 18.5 17 17.15 17 15.5V14.5H12.75C12.61 14.5 12.5 14.61 12.5 14.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16 22.75H8C4.56 22.75 2.25 20.44 2.25 17V7C2.25 3.56 4.56 1.25 8 1.25H12.93C14.47 1.25 15.91 1.85 17 2.93L20.07 6C21.16 7.09 21.75 8.53 21.75 10.07V17C21.75 20.44 19.44 22.75 16 22.75ZM8 2.75C5.42 2.75 3.75 4.42 3.75 7V17C3.75 19.58 5.42 21.25 8 21.25H16C18.58 21.25 20.25 19.58 20.25 17V10.07C20.25 8.94 19.81 7.87 19 7.06L15.93 4C15.13 3.2 14.06 2.75 12.92 2.75H8Z" fill="{color}"/>
<path d="M14 19.25H10C7.93 19.25 6.25 17.57 6.25 15.5V12.5C6.25 10.43 7.93 8.75 10 8.75H14C16.07 8.75 17.75 10.43 17.75 12.5V15.5C17.75 17.57 16.07 19.25 14 19.25ZM10 10.25C8.76 10.25 7.75 11.26 7.75 12.5V15.5C7.75 16.74 8.76 17.75 10 17.75H14C15.24 17.75 16.25 16.74 16.25 15.5V12.5C16.25 11.26 15.24 10.25 14 10.25H10Z" fill="{color}"/>
<path d="M12 19.25C11.59 19.25 11.25 18.91 11.25 18.5V9.5C11.25 9.09 11.59 8.75 12 8.75C12.41 8.75 12.75 9.09 12.75 9.5V18.5C12.75 18.91 12.41 19.25 12 19.25Z" fill="{color}"/>
<path d="M16.5 14.75H7.5C7.09 14.75 6.75 14.41 6.75 14C6.75 13.59 7.09 13.25 7.5 13.25H16.5C16.91 13.25 17.25 13.59 17.25 14C17.25 14.41 16.91 14.75 16.5 14.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M19.54 6.54L16.47 3.47C15.53 2.53 14.26 2 12.93 2H8C5 2 3 4 3 7V17C3 20 5 22 8 22H16C19 22 21 20 21 17V10.07C21 8.74 20.47 7.47 19.54 6.54Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<g opacity="0.4">
<path d="M10 18.5H14C15.65 18.5 17 17.15 17 15.5V12.5C17 10.85 15.65 9.5 14 9.5H10C8.35 9.5 7 10.85 7 12.5V15.5C7 17.15 8.35 18.5 10 18.5Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 9.5V18.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7.5 14H16.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</g>
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