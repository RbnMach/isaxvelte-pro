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
<path d="M16.5 8.89995L12 6.19995L7.5 8.89995" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7.5 9V15.1L12 12.4L16.5 15.1V9" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M14.2 16.2L12 17.7L9.80005 16.2" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM14.67 16.43L12.42 17.93C12.29 18.01 12.15 18.06 12 18.06C11.85 18.06 11.71 18.02 11.58 17.93L9.33 16.43C8.99 16.2 8.89 15.73 9.12 15.39C9.35 15.04 9.82 14.95 10.16 15.18L11.99 16.4L13.82 15.18C14.16 14.95 14.63 15.04 14.86 15.39C15.1 15.74 15.01 16.2 14.67 16.43ZM16.5 12.99C16.5 13.77 15.65 14.25 14.99 13.85L12.52 12.37C12.2 12.18 11.81 12.18 11.49 12.37L9.02 13.85C8.35 14.25 7.50999 13.77 7.50999 12.99V9.16C7.50999 8.82 7.69 8.50001 7.97 8.32001L11.47 6.10001C11.8 5.89001 12.21 5.89001 12.54 6.10001L16.04 8.32001C16.33 8.50001 16.5 8.82 16.5 9.16V12.99Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.5 8.84991L12 6.1499L7.5 8.84991" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16.5 11.19V9" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7.5 9V15.15L12 12.45L16.5 15.15" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M14.25 16.2L12 17.7L9.75 16.2" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.2 2.30001 7.97 2.85001" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M22 12.213v5.107c0 1.040-1.133 1.68-2.013 1.147l-3.293-1.973c-0.427-0.253-0.947-0.253-1.373 0l-3.293 1.973c-0.893 0.533-2.013-0.107-2.013-1.147v-5.107c0-0.453 0.24-0.88 0.613-1.12l4.667-2.96c0.44-0.28 0.987-0.28 1.427 0l4.667 2.96c0.373 0.24 0.613 0.667 0.613 1.12z"></path>
<path fill="{color}" d="M16.001 24.080c-0.2 0-0.387-0.053-0.56-0.173l-3-2c-0.453-0.307-0.587-0.933-0.28-1.387 0.307-0.467 0.933-0.587 1.387-0.28l2.44 1.627 2.44-1.627c0.453-0.307 1.080-0.187 1.387 0.28 0.307 0.453 0.187 1.080-0.28 1.387l-3 2c-0.147 0.12-0.333 0.173-0.533 0.173z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.4999 9.60003C16.3699 9.60003 16.2399 9.57002 16.1099 9.49003L11.9999 7.02002L7.88988 9.49003C7.53988 9.70003 7.06988 9.59002 6.85988 9.23002C6.64988 8.88002 6.75988 8.41002 7.11988 8.20002L11.6199 5.50002C11.8599 5.36002 12.1499 5.36002 12.3899 5.50002L16.8899 8.20002C17.2499 8.41002 17.3599 8.87002 17.1499 9.23002C16.9999 9.47002 16.7499 9.60003 16.4999 9.60003Z" fill="{color}"/>
<path d="M16.5 15.9C16.37 15.9 16.23 15.86 16.11 15.79L12 13.32L7.89 15.79C7.66 15.93 7.37 15.93 7.13 15.8C6.9 15.67 6.75 15.42 6.75 15.15V9C6.75 8.59 7.09 8.25 7.5 8.25C7.91 8.25 8.25 8.59 8.25 9V13.83L11.61 11.81C11.85 11.67 12.14 11.67 12.38 11.81L15.74 13.83V9C15.74 8.59 16.08 8.25 16.49 8.25C16.9 8.25 17.24 8.59 17.24 9V15.15C17.24 15.42 17.09 15.67 16.86 15.8C16.75 15.87 16.63 15.9 16.5 15.9Z" fill="{color}"/>
<path d="M12.0004 18.4498C11.8504 18.4498 11.7104 18.4098 11.5804 18.3198L9.33044 16.8198C8.99044 16.5898 8.89043 16.1198 9.12043 15.7798C9.35043 15.4298 9.82044 15.3398 10.1604 15.5698L11.9904 16.7898L13.8204 15.5698C14.1604 15.3398 14.6304 15.4298 14.8604 15.7798C15.0904 16.1198 15.0004 16.5898 14.6504 16.8198L12.4004 18.3198C12.2904 18.4098 12.1504 18.4498 12.0004 18.4498Z" fill="{color}"/>
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<g opacity="0.4">
<path d="M16.5 8.84991L12 6.1499L7.5 8.84991" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7.5 9V15.15L12 12.45L16.5 15.15V9" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</g>
<path opacity="0.4" d="M14.25 16.2002L12 17.7002L9.75 16.2002" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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