<script lang="ts">
	export let color = 'currentColor';
	export let variant: 'linear' | 'bold' | 'broken' | 'bulk' | 'outline' | 'twotone' = 'linear';
	export let size = '1.1em';
	export let axis_y = '-0.13em';
	export let axis_x = '0';
	export let flip_x = false;
	export let flip_y = false;
	export let rotate = 0;	
</script>

<span style="width: {size}; height: {size}; bottom: {axis_y}; left: {axis_x}; transform: rotate({rotate}deg);" class:horizontal-reverted={flip_x} class:vertical-reverted={flip_y}>
	{#if variant == 'linear'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path fill-rule="evenodd" clip-rule="evenodd" d="M6 9.70005V12.5C6 14 7.3 15.3 8.8 15.3H12.5C13 15.3 13.4 14.9 13.4 14.4V11.6C13.4 10.1 12.2 8.80005 10.6 8.80005H6.9C6.4 8.80005 6 9.20005 6 9.70005Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path fill-rule="evenodd" clip-rule="evenodd" d="M18 9.19995V14.8L15.2 12.9V11.1L18 9.19995Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM13.63 14.29C13.63 14.8 13.22 15.21 12.71 15.21L9.03 15.24C7.49 15.25 6.23999 14.01 6.23999 12.47V9.67001C6.23999 9.16001 6.65 8.75 7.16 8.75H10.85C12.38 8.75 13.62 9.98999 13.62 11.52V14.29H13.63ZM17.75 14C17.75 14.43 17.27 14.69 16.91 14.45L14.99 13.17C14.84 13.07 14.75 12.9 14.75 12.72V11.3C14.75 11.12 14.84 10.95 14.99 10.85L16.91 9.57001C17.27 9.33001 17.75 9.58999 17.75 10.02V14Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path fill-rule="evenodd" clip-rule="evenodd" d="M6 9.67999V12.48C6 14.02 7.25001 15.26 8.79001 15.25L12.47 15.22C12.98 15.22 13.39 14.8 13.39 14.3V11.53C13.39 10 12.15 8.76001 10.62 8.76001H6.92999C6.40999 8.76001 6 9.16999 6 9.67999Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path fill-rule="evenodd" clip-rule="evenodd" d="M18.0005 9.23999V14.78L15.2305 12.93V11.09L18.0005 9.23999Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.2 2.30001 7.97 2.85001" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M8.333 12.906v3.733c0 2.053 1.667 3.707 3.72 3.693l4.907-0.040c0.68 0 1.227-0.56 1.227-1.227v-3.693c0-2.040-1.653-3.693-3.693-3.693h-4.92c-0.693 0-1.24 0.547-1.24 1.227z"></path>
<path fill="{color}" d="M23.667 13.359v5.307c0 0.573-0.64 0.92-1.12 0.6l-2.56-1.707c-0.2-0.133-0.32-0.36-0.32-0.6v-1.893c0-0.24 0.12-0.467 0.32-0.6l2.56-1.707c0.48-0.32 1.12 0.027 1.12 0.6z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M8.76999 15.99C7.83999 15.99 6.96001 15.63 6.29001 14.97C5.62001 14.3 5.25 13.42 5.25 12.47V9.67001C5.25 8.75001 6.00001 8 6.92001 8H10.61C12.55 8 14.13 9.57999 14.13 11.52V14.29C14.13 15.21 13.38 15.96 12.47 15.96L8.79001 15.99C8.79001 15.99 8.77999 15.99 8.76999 15.99ZM6.92001 9.51001C6.82001 9.51001 6.75 9.58999 6.75 9.67999V12.48C6.75 13.02 6.96001 13.53 7.35001 13.91C7.73001 14.29 8.25001 14.53 8.79001 14.5L12.47 14.47C12.56 14.47 12.64 14.39 12.64 14.3V11.53C12.64 10.42 11.73 9.51001 10.62 9.51001H6.92001Z" fill="{color}"/>
<path d="M18.0005 15.5301C17.8505 15.5301 17.7104 15.4901 17.5804 15.4001L14.8105 13.5501C14.6005 13.4101 14.4805 13.1801 14.4805 12.9301V11.0801C14.4805 10.8301 14.6105 10.5901 14.8105 10.4601L17.5804 8.61008C17.8104 8.46008 18.1105 8.4401 18.3505 8.5701C18.5905 8.7001 18.7505 8.9501 18.7505 9.2301V14.7701C18.7505 15.0501 18.6005 15.3001 18.3505 15.4301C18.2405 15.5001 18.1205 15.5301 18.0005 15.5301ZM15.9805 12.5301L17.2505 13.3801V10.6401L15.9805 11.4901V12.5301Z" fill="{color}"/>
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" fill-rule="evenodd" clip-rule="evenodd" d="M6 9.67975V12.4798C6 14.0198 7.25001 15.2598 8.79001 15.2498L12.47 15.2198C12.98 15.2198 13.39 14.7997 13.39 14.2997V11.5298C13.39 9.99975 12.15 8.75977 10.62 8.75977H6.92999C6.40999 8.75977 6 9.16975 6 9.67975Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path opacity="0.4" fill-rule="evenodd" clip-rule="evenodd" d="M18.0005 9.24023V14.7802L15.2305 12.9302V11.0902L18.0005 9.24023Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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
	.horizontal-reverted {
		transform: scale(-1, 1);
	}
	.vertical-reverted {
		transform: scale(1, -1);
	}
</style>