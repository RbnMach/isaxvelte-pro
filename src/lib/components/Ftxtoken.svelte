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
<path d="M21 2H9C8.4 2 8 2.4 8 3V6C8 6.6 8.4 7 9 7H21C21.6 7 22 6.6 22 6V3C22 2.4 21.6 2 21 2Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 17H7V22H12V17Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7 9.5H2V14.5H7V9.5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M18 9.6001H9.5V14.3001H18V9.6001Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M21 2H9C8.45 2 8 2.45 8 3V6C8 6.55 8.45 7 9 7H21C21.55 7 22 6.55 22 6V3C22 2.45 21.55 2 21 2Z" fill="{color}"/>
<path d="M11 17H8C7.45 17 7 17.45 7 18V21C7 21.55 7.45 22 8 22H11C11.55 22 12 21.55 12 21V18C12 17.45 11.55 17 11 17Z" fill="{color}"/>
<path d="M6 9.5H3C2.45 9.5 2 9.95 2 10.5V13.5C2 14.05 2.45 14.5 3 14.5H6C6.55 14.5 7 14.05 7 13.5V10.5C7 9.95 6.55 9.5 6 9.5Z" fill="{color}"/>
<path d="M17 9.64062H10.5C9.95 9.64062 9.5 10.0906 9.5 10.6406V13.3606C9.5 13.9106 9.95 14.3606 10.5 14.3606H17C17.55 14.3606 18 13.9106 18 13.3606V10.6406C18 10.0906 17.55 9.64062 17 9.64062Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M21 2H9C8.45 2 8 2.45 8 3V6C8 6.55 8.45 7 9 7H21C21.55 7 22 6.55 22 6V3C22 2.45 21.55 2 21 2Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 17H7V22H12V17Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7 9.5H2V14.5H7V9.5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17 14.3599H18V9.63989H9.5V14.3599H12.92" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" d="M28 2.667h-16c-0.733 0-1.333 0.6-1.333 1.333v4c0 0.733 0.6 1.333 1.333 1.333h16c0.733 0 1.333-0.6 1.333-1.333v-4c0-0.733-0.6-1.333-1.333-1.333z"></path>
<path fill="{color}" d="M14.667 22.667h-4c-0.733 0-1.333 0.6-1.333 1.333v4c0 0.733 0.6 1.333 1.333 1.333h4c0.733 0 1.333-0.6 1.333-1.333v-4c0-0.733-0.6-1.333-1.333-1.333z"></path>
<path fill="{color}" opacity="0.4" d="M8 12.667h-4c-0.733 0-1.333 0.6-1.333 1.333v4c0 0.733 0.6 1.333 1.333 1.333h4c0.733 0 1.333-0.6 1.333-1.333v-4c0-0.733-0.6-1.333-1.333-1.333z"></path>
<path fill="{color}" opacity="0.4" d="M22.667 12.854h-8.667c-0.733 0-1.333 0.6-1.333 1.333v3.627c0 0.733 0.6 1.333 1.333 1.333h8.667c0.733 0 1.333-0.6 1.333-1.333v-3.627c0-0.733-0.6-1.333-1.333-1.333z"></path>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M21 7.75H9C8.04 7.75 7.25 6.96 7.25 6V3C7.25 2.04 8.04 1.25 9 1.25H21C21.96 1.25 22.75 2.04 22.75 3V6C22.75 6.96 21.96 7.75 21 7.75ZM9 2.75C8.86 2.75 8.75 2.86 8.75 3V6C8.75 6.14 8.86 6.25 9 6.25H21C21.14 6.25 21.25 6.14 21.25 6V3C21.25 2.86 21.14 2.75 21 2.75H9Z" fill="{color}"/>
<path d="M12 22.75H7C6.59 22.75 6.25 22.41 6.25 22V17C6.25 16.59 6.59 16.25 7 16.25H12C12.41 16.25 12.75 16.59 12.75 17V22C12.75 22.41 12.41 22.75 12 22.75ZM7.75 21.25H11.25V17.75H7.75V21.25Z" fill="{color}"/>
<path d="M7 15.25H2C1.59 15.25 1.25 14.91 1.25 14.5V9.5C1.25 9.09 1.59 8.75 2 8.75H7C7.41 8.75 7.75 9.09 7.75 9.5V14.5C7.75 14.91 7.41 15.25 7 15.25ZM2.75 13.75H6.25V10.25H2.75V13.75Z" fill="{color}"/>
<path d="M18 15.1101H9.5C9.09 15.1101 8.75 14.7701 8.75 14.3601V9.64014C8.75 9.23014 9.09 8.89014 9.5 8.89014H18C18.41 8.89014 18.75 9.23014 18.75 9.64014V14.3601C18.75 14.7801 18.41 15.1101 18 15.1101ZM10.25 13.6101H17.25V10.3901H10.25V13.6101Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M21 2H9C8.45 2 8 2.45 8 3V6C8 6.55 8.45 7 9 7H21C21.55 7 22 6.55 22 6V3C22 2.45 21.55 2 21 2Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 17H7V22H12V17Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M7 9.5H2V14.5H7V9.5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M18 9.64014H9.5V14.3601H18V9.64014Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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