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
<path d="M11.6 6.3999H14.1L12 14.2999H16.2L15.7 17.0999H8L11 6.3999H11.6Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15 11L7.30005 12.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM15.82 16.32C15.73 16.8 15.32 17.14 14.84 17.14H9.29999C8.63999 17.14 8.16 16.5 8.34 15.87L9.17999 12.92L7.47 13.26C7.42 13.27 7.37001 13.27 7.32001 13.27C6.97001 13.27 6.66 13.02 6.59 12.67C6.51 12.26 6.76999 11.87 7.17999 11.79L9.64999 11.3L10.96 6.73C11.02 6.52 11.22 6.37 11.44 6.37H12.8C13.46 6.37 13.94 6.99 13.77 7.63L12.96 10.64L14.89 10.25C15.29 10.17 15.69 10.43 15.77 10.84C15.85 11.25 15.59 11.64 15.18 11.72L12.52 12.25L11.97 14.3H15C15.62 14.3 16.09 14.86 15.98 15.48L15.82 16.32Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11.5607 6.36011H14.0907L11.9607 14.3001H16.1807L15.6707 17.1401H7.9707L11.0507 6.36011H11.5607Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.0203 10.98L7.32031 12.52" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.2 2.3 7.97 2.85" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M17.041 8.48c0.88 0 1.52 0.827 1.293 1.68l-2.387 8.907h4.040c0.827 0 1.467 0.747 1.307 1.573l-0.2 1.12c-0.12 0.64-0.667 1.093-1.307 1.093h-7.387c-0.88 0-1.52-0.853-1.28-1.693l3.48-12.187c0.080-0.28 0.347-0.48 0.64-0.48h1.8v-0.013z"></path>
<path fill="{color}" d="M9.761 17.693c-0.467 0-0.88-0.333-0.973-0.8-0.107-0.547 0.24-1.067 0.787-1.173l10.267-2.053c0.533-0.107 1.067 0.24 1.173 0.787s-0.24 1.067-0.787 1.173l-10.267 2.053c-0.067 0.013-0.133 0.013-0.2 0.013z"></path>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15.6702 17.8899H7.97017C7.73017 17.8899 7.51016 17.7799 7.37016 17.5899C7.23016 17.3999 7.18016 17.1599 7.25016 16.9299L10.3302 6.14986C10.4202 5.82986 10.7202 5.60986 11.0502 5.60986H14.0902C14.3202 5.60986 14.5402 5.71986 14.6902 5.89986C14.8302 6.08986 14.8802 6.32987 14.8202 6.54987L12.9502 13.5499H16.2002C16.4202 13.5499 16.6302 13.6499 16.7802 13.8199C16.9202 13.9899 16.9802 14.2199 16.9402 14.4299L16.4302 17.2699C16.3402 17.6299 16.0302 17.8899 15.6702 17.8899ZM8.96016 16.3899H15.0402L15.2802 15.0499H11.9602C11.7302 15.0499 11.5101 14.9399 11.3601 14.7599C11.2201 14.5699 11.1702 14.3299 11.2302 14.1099L13.1002 7.10986H11.6002L8.96016 16.3899Z" fill="{color}"/>
<path d="M7.31965 13.2698C6.96965 13.2698 6.65964 13.0198 6.58964 12.6698C6.50964 12.2598 6.76964 11.8698 7.17964 11.7898L14.8796 10.2498C15.2796 10.1698 15.6797 10.4298 15.7597 10.8398C15.8397 11.2498 15.5797 11.6398 15.1697 11.7198L7.46964 13.2598C7.41964 13.2698 7.36965 13.2698 7.31965 13.2698Z" fill="{color}"/>
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<g opacity="0.4">
<path d="M11.5607 6.35986H14.0907L11.9607 14.2999H16.1807L15.6707 17.1399H7.9707L11.0507 6.35986H11.5607Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.0203 10.98L7.32031 12.52" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</g>
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
</style>