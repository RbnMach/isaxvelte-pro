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
<path d="M20.2 3.80005H20.2999" stroke="{color}" stroke-width="3" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3.69995 20.2H3.79995" stroke="{color}" stroke-width="3" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.6 6C14.5 5.4 13.3 5 12 5C8.1 5 5 8.1 5 12C5 13.3 5.4 14.6 6 15.7" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.30005 18C9.40005 18.7 10.6 19 12 19C15.9 19 19 15.9 19 12C19 10.7 18.6 9.40005 18 8.30005" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M20.2598 5.25C19.4298 5.25 18.7598 4.58 18.7598 3.75C18.7598 2.92 19.4298 2.25 20.2598 2.25H20.2697C21.0997 2.25 21.7697 2.92 21.7697 3.75C21.7697 4.58 21.0898 5.25 20.2598 5.25Z" fill="{color}"/>
<path d="M3.75977 21.75C2.92977 21.75 2.25977 21.08 2.25977 20.25C2.25977 19.42 2.92977 18.75 3.75977 18.75H3.76974C4.59974 18.75 5.26974 19.42 5.26974 20.25C5.26974 21.08 4.58977 21.75 3.75977 21.75Z" fill="{color}"/>
<path d="M6.03 16.4C5.78 16.4 5.53001 16.27 5.39001 16.04C4.65001 14.83 4.25 13.43 4.25 12C4.25 7.73 7.73 4.25 12 4.25C13.41 4.25 14.79 4.63001 15.99 5.35001C16.34 5.56001 16.46 6.02 16.25 6.38C16.04 6.73 15.58 6.85 15.22 6.64C14.25 6.06 13.14 5.75 12.01 5.75C8.56001 5.75 5.76001 8.55 5.76001 12C5.76001 13.15 6.07999 14.28 6.67999 15.26C6.89999 15.61 6.78999 16.07 6.42999 16.29C6.29999 16.37 6.16 16.4 6.03 16.4Z" fill="{color}"/>
<path d="M12.0001 19.7503C10.5601 19.7503 9.16013 19.3503 7.95013 18.6103C7.60013 18.3903 7.49013 17.9303 7.70013 17.5803C7.92013 17.2303 8.38012 17.1203 8.73012 17.3303C9.71012 17.9303 10.8401 18.2503 12.0001 18.2503C15.4501 18.2503 18.2501 15.4503 18.2501 12.0003C18.2501 10.8503 17.9301 9.72028 17.3301 8.74028C17.1101 8.39028 17.2201 7.93028 17.5801 7.71028C17.9301 7.50028 18.3901 7.60028 18.6101 7.96028C19.3501 9.18028 19.7501 10.5703 19.7501 12.0103C19.7501 16.2703 16.2701 19.7503 12.0001 19.7503Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M20.1992 3.80005H20.2992" stroke="{color}" stroke-width="3" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M3.69922 20.2H3.79922" stroke="{color}" stroke-width="3" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.6 6C14.55 5.37 13.32 5 12 5C8.13 5 5 8.13 5 12C5 13.34 5.38 14.59 6.03 15.65" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17.9707 8.3501C18.6207 9.4101 19.0007 10.6601 19.0007 12.0001C19.0007 13.2401 18.6807 14.4001 18.1107 15.4101" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.33984 17.97C9.40984 18.62 10.6598 19 11.9998 19C13.0498 19 14.0499 18.77 14.9499 18.35" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M27.013 7c-1.107 0-2-0.893-2-2s0.893-2 2-2h0.013c1.107 0 2 0.893 2 2s-0.907 2-2.013 2z"></path>
<path fill="{color}" opacity="0.4" d="M5.013 29c-1.107 0-2-0.893-2-2s0.893-2 2-2h0.013c1.107 0 2 0.893 2 2s-0.907 2-2.013 2z"></path>
<path fill="{color}" d="M8.040 21.867c-0.333 0-0.667-0.173-0.853-0.48-0.987-1.613-1.52-3.48-1.52-5.387 0-5.693 4.64-10.333 10.333-10.333 1.88 0 3.72 0.507 5.32 1.467 0.467 0.28 0.627 0.893 0.347 1.373-0.28 0.467-0.893 0.627-1.373 0.347-1.293-0.773-2.773-1.187-4.28-1.187-4.6 0-8.333 3.733-8.333 8.333 0 1.533 0.427 3.040 1.227 4.347 0.293 0.467 0.147 1.080-0.333 1.373-0.173 0.107-0.36 0.147-0.533 0.147z"></path>
<path fill="{color}" d="M16 26.334c-1.92 0-3.787-0.533-5.4-1.52-0.467-0.293-0.613-0.907-0.333-1.373 0.293-0.467 0.907-0.613 1.373-0.333 1.307 0.8 2.813 1.227 4.36 1.227 4.6 0 8.333-3.733 8.333-8.333 0-1.533-0.427-3.040-1.227-4.347-0.293-0.467-0.147-1.080 0.333-1.373 0.467-0.28 1.080-0.147 1.373 0.333 0.987 1.627 1.52 3.48 1.52 5.4 0 5.68-4.64 10.32-10.333 10.32z"></path>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M20.2598 5.25C19.4298 5.25 18.7598 4.58 18.7598 3.75C18.7598 2.92 19.4298 2.25 20.2598 2.25H20.2697C21.0997 2.25 21.7697 2.92 21.7697 3.75C21.7697 4.58 21.0898 5.25 20.2598 5.25Z" fill="{color}"/>
<path d="M3.75977 21.75C2.92977 21.75 2.25977 21.08 2.25977 20.25C2.25977 19.42 2.92977 18.75 3.75977 18.75H3.76974C4.59974 18.75 5.26974 19.42 5.26974 20.25C5.26974 21.08 4.58977 21.75 3.75977 21.75Z" fill="{color}"/>
<path d="M6.03 16.4C5.78 16.4 5.53001 16.27 5.39001 16.04C4.65001 14.83 4.25 13.43 4.25 12C4.25 7.73 7.73 4.25 12 4.25C13.41 4.25 14.79 4.63001 15.99 5.35001C16.34 5.56001 16.46 6.02 16.25 6.38C16.04 6.73 15.58 6.85 15.22 6.64C14.25 6.06 13.14 5.75 12.01 5.75C8.56001 5.75 5.76001 8.55 5.76001 12C5.76001 13.15 6.07999 14.28 6.67999 15.26C6.89999 15.61 6.78999 16.07 6.42999 16.29C6.29999 16.37 6.16 16.4 6.03 16.4Z" fill="{color}"/>
<path d="M12.0001 19.7498C10.5601 19.7498 9.16013 19.3498 7.95013 18.6098C7.60013 18.3898 7.49013 17.9298 7.70013 17.5798C7.92013 17.2298 8.38012 17.1198 8.73012 17.3298C9.71012 17.9298 10.8401 18.2498 12.0001 18.2498C15.4501 18.2498 18.2501 15.4498 18.2501 11.9998C18.2501 10.8498 17.9301 9.71979 17.3301 8.73979C17.1101 8.38979 17.2201 7.92979 17.5801 7.70979C17.9301 7.49979 18.3901 7.59979 18.6101 7.95979C19.3501 9.1798 19.7501 10.5698 19.7501 12.0098C19.7501 16.2698 16.2701 19.7498 12.0001 19.7498Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15.6 6C14.55 5.37 13.32 5 12 5C8.13 5 5 8.13 5 12C5 13.34 5.38 14.59 6.03 15.65" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.33984 17.9701C9.40984 18.6201 10.6598 19.0001 11.9998 19.0001C15.8698 19.0001 18.9998 15.8701 18.9998 12.0001C18.9998 10.6601 18.6198 9.4101 17.9698 8.3501" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M20.2002 3.7998H20.3002" stroke="{color}" stroke-width="3" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M3.7002 20.2002H3.8002" stroke="{color}" stroke-width="3" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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