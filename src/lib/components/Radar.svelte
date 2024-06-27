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
<path d="M6 4C7.67 2.75 9.75 2 12 2C17.52 2 22 6.48 22 12C22 17.52 17.52 22 12 22C6.48 22 2 17.52 2 12C2 10.19 2.47999 8.48999 3.32999 7.01999L12 12" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM12 19.75C7.73 19.75 4.25 16.27 4.25 12C4.25 10.64 4.61 9.31 5.28 8.14C5.48 7.78 5.94 7.66 6.3 7.86L12.37 11.35C12.73 11.56 12.85 12.01 12.65 12.37C12.44 12.73 11.99 12.85 11.63 12.65L6.24 9.56C5.92 10.33 5.75 11.16 5.75 12C5.75 15.45 8.55 18.25 12 18.25C15.45 18.25 18.25 15.45 18.25 12C18.25 8.55 15.45 5.75 12 5.75C10.64 5.75 9.34 6.18 8.25 7C7.92 7.25 7.45 7.18 7.2 6.85C6.95 6.52 7.02 6.05 7.35 5.8C8.7 4.79 10.31 4.25 12 4.25C16.27 4.25 19.75 7.73 19.75 12C19.75 16.27 16.27 19.75 12 19.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M20.32 6.45996C21.38 8.04996 22 9.94997 22 12C22 17.52 17.52 22 12 22C6.48 22 2 17.52 2 12C2 10.19 2.47999 8.48996 3.32999 7.01996L12 12" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6 4C7.67 2.75 9.75 2 12 2C13.93 2 15.73 2.53999 17.25 3.48999" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" fill="{color}"/>
<path d="M12 19.75C7.73 19.75 4.25 16.27 4.25 12C4.25 10.64 4.61 9.31 5.28 8.14C5.49 7.78 5.94999 7.66 6.29999 7.86L12.37 11.35C12.73 11.56 12.85 12.01 12.65 12.37C12.44 12.73 11.99 12.85 11.63 12.65L6.25 9.56C5.93 10.33 5.76001 11.16 5.76001 12C5.76001 15.45 8.56001 18.25 12.01 18.25C15.46 18.25 18.26 15.45 18.26 12C18.26 8.55 15.46 5.75 12.01 5.75C10.65 5.75 9.35001 6.18 8.26001 7C7.93001 7.25 7.45999 7.18001 7.20999 6.85001C6.95999 6.52001 7.02999 6.05 7.35999 5.8C8.70999 4.79 10.32 4.25 12.01 4.25C16.28 4.25 19.76 7.73 19.76 12C19.76 16.27 16.27 19.75 12 19.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22.7502C6.07 22.7502 1.25 17.9302 1.25 12.0002C1.25 10.1202 1.73999 8.27026 2.67999 6.64026C2.88999 6.28026 3.34001 6.16023 3.70001 6.36023L12.37 11.3402C12.73 11.5502 12.85 12.0002 12.65 12.3602C12.44 12.7202 11.99 12.8403 11.63 12.6403L3.63 8.05023C3.05 9.28023 2.75 10.6202 2.75 11.9902C2.75 17.0902 6.9 21.2402 12 21.2402C17.1 21.2402 21.25 17.0902 21.25 11.9902C21.25 6.89023 17.1 2.74023 12 2.74023C9.98 2.74023 8.06001 3.38024 6.45001 4.59024C6.12001 4.84024 5.64999 4.77025 5.39999 4.44025C5.14999 4.11025 5.21999 3.64026 5.54999 3.39026C7.41999 1.99026 9.65 1.24023 12 1.24023C17.93 1.24023 22.75 6.06023 22.75 11.9902C22.75 17.9202 17.93 22.7502 12 22.7502Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M6 4C7.67 2.75 9.75 2 12 2C17.52 2 22 6.48 22 12C22 17.52 17.52 22 12 22C6.48 22 2 17.52 2 12C2 10.19 2.47999 8.48999 3.32999 7.01999L12 12" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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