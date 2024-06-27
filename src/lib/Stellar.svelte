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
<path d="M16.3998 5.00005C15.0998 4.20005 13.5998 3.80005 11.9998 3.80005C7.3998 3.80005 3.7998 7.50005 3.7998 12C3.7998 12.8 3.8998 13.5 4.0998 14.2" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7.6001 19C8.9001 19.8 10.4001 20.3 12.0001 20.3C16.6001 20.3 20.2001 16.6 20.2001 12.1C20.2001 11.3 20.1001 10.5 19.9001 9.69995" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 16L22 5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M22 8.5L2 19.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M22.6595 4.64C22.4595 4.28 21.9996 4.14 21.6396 4.34L4.69959 13.66C4.57959 13.12 4.49958 12.56 4.49958 12C4.49958 7.86 7.85958 4.5 11.9996 4.5C13.4096 4.5 14.7796 4.89 15.9596 5.63C16.3096 5.85 16.7696 5.74 16.9896 5.39C17.2096 5.04 17.0996 4.58 16.7496 4.36C15.3296 3.47 13.6896 3 11.9996 3C7.03958 3 2.99958 7.04 2.99958 12C2.99958 12.81 3.10958 13.61 3.31958 14.39C3.31958 14.4 3.32959 14.4 3.32959 14.41L1.63959 15.34C1.27959 15.54 1.1396 16 1.3396 16.36C1.4796 16.61 1.72958 16.75 1.99958 16.75C2.11958 16.75 2.24956 16.72 2.35956 16.66L22.3596 5.66C22.7196 5.46 22.8596 5 22.6595 4.64Z" fill="{color}"/>
<path d="M22.6595 8.14156C22.4595 7.78156 21.9996 7.64155 21.6396 7.84155L19.5296 9.00156C19.4996 9.02156 19.4596 9.03155 19.4296 9.06155L1.63959 18.8416C1.27959 19.0416 1.1396 19.5016 1.3396 19.8616C1.4796 20.1116 1.72958 20.2516 1.99958 20.2516C2.11958 20.2516 2.24956 20.2216 2.35956 20.1616L19.3896 10.7916C19.4496 11.1916 19.4996 11.5916 19.4996 12.0016C19.4996 16.1416 16.1396 19.5016 11.9996 19.5016C10.5796 19.5016 9.2096 19.1016 8.0196 18.3616C7.6696 18.1416 7.20957 18.2516 6.98957 18.6016C6.76957 18.9516 6.86956 19.4116 7.22956 19.6316C8.65956 20.5316 10.3096 21.0016 12.0096 21.0016C16.9696 21.0016 21.0096 16.9616 21.0096 12.0016C21.0096 11.3316 20.9096 10.6816 20.7696 10.0416L22.3696 9.16156C22.7196 8.96156 22.8596 8.50156 22.6595 8.14156Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.36 4.99C15.1 4.2 13.6 3.75 12 3.75C7.44 3.75 3.75 7.44 3.75 12C3.75 12.76 3.84998 13.49 4.03998 14.19" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7.61914 18.9899C8.88914 19.7899 10.3891 20.2499 11.9991 20.2499C16.5591 20.2499 20.2491 16.5599 20.2491 11.9999C20.2491 11.1799 20.1291 10.3799 19.9091 9.63989" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M13.9297 9.44L21.9997 5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 16.0001L10.05 11.5701" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M22 8.5L2 19.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" d="M30.213 6.187c-0.267-0.48-0.88-0.667-1.36-0.4l-22.587 12.427c-0.16-0.72-0.267-1.467-0.267-2.213 0-5.52 4.48-10 10-10 1.88 0 3.707 0.52 5.28 1.507 0.467 0.293 1.080 0.147 1.373-0.32s0.147-1.080-0.32-1.373c-1.893-1.187-4.080-1.813-6.333-1.813-6.613 0-12 5.387-12 12 0 1.080 0.147 2.147 0.427 3.187 0 0.013 0.013 0.013 0.013 0.027l-2.253 1.24c-0.48 0.267-0.667 0.88-0.4 1.36 0.187 0.333 0.52 0.52 0.88 0.52 0.16 0 0.333-0.040 0.48-0.12l26.667-14.667c0.48-0.267 0.667-0.88 0.4-1.36z"></path>
<path fill="{color}" opacity="0.4" d="M30.213 10.853c-0.267-0.48-0.88-0.667-1.36-0.4l-2.813 1.547c-0.040 0.027-0.093 0.040-0.133 0.080l-23.72 13.040c-0.48 0.267-0.667 0.88-0.4 1.36 0.187 0.333 0.52 0.52 0.88 0.52 0.16 0 0.333-0.040 0.48-0.12l22.707-12.493c0.080 0.533 0.147 1.067 0.147 1.613 0 5.52-4.48 10-10 10-1.893 0-3.72-0.533-5.307-1.52-0.467-0.293-1.080-0.147-1.373 0.32s-0.16 1.080 0.32 1.373c1.907 1.2 4.107 1.827 6.373 1.827 6.613 0 12-5.387 12-12 0-0.893-0.133-1.76-0.32-2.613l2.133-1.173c0.467-0.267 0.653-0.88 0.387-1.36z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M4.03998 14.94C3.70998 14.94 3.41001 14.72 3.32001 14.39C3.11001 13.61 3 12.81 3 12C3 7.04 7.04 3 12 3C13.69 3 15.33 3.47 16.75 4.36C17.1 4.58 17.21 5.04 16.99 5.39C16.77 5.74 16.31 5.85 15.96 5.63C14.77 4.89 13.4 4.5 12 4.5C7.86 4.5 4.5 7.86 4.5 12C4.5 12.68 4.59002 13.35 4.77002 13.99C4.88002 14.39 4.63999 14.8 4.23999 14.91C4.17999 14.93 4.10998 14.94 4.03998 14.94Z" fill="{color}"/>
<path d="M11.9998 21.0001C10.2998 21.0001 8.64979 20.5201 7.21979 19.6301C6.86979 19.4101 6.7598 18.9501 6.9798 18.6001C7.1998 18.2501 7.65983 18.1401 8.00983 18.3601C9.19983 19.1101 10.5798 19.5001 11.9898 19.5001C16.1298 19.5001 19.4898 16.1401 19.4898 12.0001C19.4898 11.2701 19.3798 10.5401 19.1798 9.85007C19.0598 9.45007 19.2898 9.04007 19.6798 8.92007C20.0798 8.80007 20.4898 9.03007 20.6098 9.42007C20.8598 10.2501 20.9898 11.1201 20.9898 12.0001C20.9998 16.9601 16.9598 21.0001 11.9998 21.0001Z" fill="{color}"/>
<path d="M1.99965 16.7502C1.73965 16.7502 1.47968 16.6102 1.33968 16.3602C1.13968 16.0002 1.26967 15.5402 1.63967 15.3402L21.6397 4.34016C21.9997 4.14016 22.4596 4.27017 22.6596 4.64017C22.8596 5.00017 22.7296 5.46017 22.3596 5.66017L2.35964 16.6602C2.24964 16.7202 2.11965 16.7502 1.99965 16.7502Z" fill="{color}"/>
<path d="M1.99965 20.2502C1.73965 20.2502 1.47968 20.1102 1.33968 19.8602C1.13968 19.5002 1.26967 19.0402 1.63967 18.8402L21.6397 7.84016C21.9997 7.64016 22.4596 7.77017 22.6596 8.14017C22.8596 8.50017 22.7296 8.96017 22.3596 9.16017L2.35964 20.1602C2.24964 20.2202 2.11965 20.2502 1.99965 20.2502Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.36 4.99C15.1 4.2 13.6 3.75 12 3.75C7.44 3.75 3.75 7.44 3.75 12C3.75 12.76 3.84998 13.49 4.03998 14.19" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 16L22 5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<g opacity="0.4">
<path d="M7.62012 18.9901C8.89012 19.7901 10.3901 20.2501 12.0001 20.2501C16.5601 20.2501 20.2501 16.5601 20.2501 12.0001C20.2501 11.1801 20.1301 10.3801 19.9101 9.64014" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M22 8.5L2 19.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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
	.horizontal-reverted {
		transform: scale(-1, 1);
	}
	.vertical-reverted {
		transform: scale(1, -1);
	}
</style>