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
<path fill-rule="evenodd" clip-rule="evenodd" d="M4.5 2H21.5V14L16.5 19H11.5L9.5 22H6.5V19H2.5V5L4.5 2Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11 7H9V13H11V7Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16 7H14V13H16V7Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path fill-rule="evenodd" clip-rule="evenodd" d="M20.5 2H5.03999C4.70999 2 4.39001 2.17001 4.21001 2.45001L2.67 4.75C2.56 4.91 2.5 5.10999 2.5 5.29999V18C2.5 18.55 2.95 19 3.5 19H5.5C6.05 19 6.5 19.45 6.5 20V21C6.5 21.55 6.95 22 7.5 22H8.96001C9.29001 22 9.60999 21.83 9.78999 21.55L11.2 19.44C11.39 19.16 11.7 18.99 12.03 18.99H16.08C16.35 18.99 16.6 18.88 16.79 18.7L21.2 14.29C21.39 14.1 21.49 13.85 21.49 13.58V3C21.5 2.45 21.05 2 20.5 2ZM10.79 12.86C10.79 13.18 10.53 13.43 10.22 13.43H9.08C8.76 13.43 8.50999 13.17 8.50999 12.86V7.14999C8.50999 6.82999 8.77 6.57999 9.08 6.57999H10.22C10.54 6.57999 10.79 6.83999 10.79 7.14999V12.86ZM16.5 12.86C16.5 13.18 16.24 13.43 15.93 13.43H14.79C14.47 13.43 14.22 13.17 14.22 12.86V7.14999C14.22 6.82999 14.48 6.57999 14.79 6.57999H15.93C16.25 6.57999 16.5 6.83999 16.5 7.14999V12.86Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2.5 7V5L4.5 2H21.5V14L16.5 19H11.5L9.5 22H6.5V19H2.5V11.61" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11 7H9V13H11V7Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16 7H14V13H16V7Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M6.72 2.667h20.613c0.733 0 1.333 0.6 1.333 1.333v14.12c0 0.36-0.147 0.693-0.387 0.947l-5.88 5.88c-0.253 0.253-0.587 0.387-0.947 0.387h-5.4c-0.44 0-0.867 0.227-1.107 0.6l-1.88 2.813c-0.253 0.373-0.667 0.6-1.107 0.6h-1.947c-0.733 0-1.333-0.6-1.333-1.333v-1.333c0-0.733-0.6-1.333-1.333-1.333h-2.667c-0.733 0-1.333-0.6-1.333-1.333v-16.933c0-0.267 0.080-0.52 0.227-0.733l2.053-3.067c0.227-0.387 0.64-0.613 1.093-0.613z"></path>
<path fill="{color}" d="M11.333 9.52v7.613c0 0.427 0.347 0.76 0.76 0.76h1.52c0.427 0 0.76-0.347 0.76-0.76v-7.613c0-0.427-0.347-0.76-0.76-0.76h-1.52c-0.413 0-0.76 0.347-0.76 0.76z"></path>
<path fill="{color}" d="M18.948 9.52v7.613c0 0.427 0.347 0.76 0.76 0.76h1.52c0.427 0 0.76-0.347 0.76-0.76v-7.613c0-0.427-0.347-0.76-0.76-0.76h-1.52c-0.413 0-0.76 0.347-0.76 0.76z"></path>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M9.5 22.75H6.5C6.09 22.75 5.75 22.41 5.75 22V19.75H2.5C2.09 19.75 1.75 19.41 1.75 19V5C1.75 4.85 1.79 4.70999 1.88 4.57999L3.88 1.57999C4.02 1.36999 4.25 1.25 4.5 1.25H21.5C21.91 1.25 22.25 1.59 22.25 2V14C22.25 14.2 22.17 14.39 22.03 14.53L17.03 19.53C16.89 19.67 16.7 19.75 16.5 19.75H11.9L10.12 22.42C9.97999 22.62 9.75 22.75 9.5 22.75ZM7.25 21.25H9.10001L10.88 18.58C11.02 18.37 11.25 18.25 11.5 18.25H16.19L20.75 13.69V2.75H4.89999L3.25 5.23001V18.25H6.5C6.91 18.25 7.25 18.59 7.25 19V21.25Z" fill="{color}"/>
<path d="M11 13.75H9C8.59 13.75 8.25 13.41 8.25 13V7C8.25 6.59 8.59 6.25 9 6.25H11C11.41 6.25 11.75 6.59 11.75 7V13C11.75 13.41 11.41 13.75 11 13.75ZM9.75 12.25H10.25V7.75H9.75V12.25Z" fill="{color}"/>
<path d="M16 13.75H14C13.59 13.75 13.25 13.41 13.25 13V7C13.25 6.59 13.59 6.25 14 6.25H16C16.41 6.25 16.75 6.59 16.75 7V13C16.75 13.41 16.41 13.75 16 13.75ZM14.75 12.25H15.25V7.75H14.75V12.25Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path fill-rule="evenodd" clip-rule="evenodd" d="M4.5 2H21.5V14L16.5 19H11.5L9.5 22H6.5V19H2.5V5L4.5 2Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M11 7H9V13H11V7Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M16 7H14V13H16V7Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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