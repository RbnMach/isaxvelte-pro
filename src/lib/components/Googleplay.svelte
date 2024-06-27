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
<path d="M21.4 12.9L16.9 15.2L13.7 12L16.9 8.80005L21.4 11C22.2 11.4 22.2 12.6 21.4 12.9Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16.9 8.79996L13.7 12L4.1 21.6L3.5 21.9C2.8 22.3 2 21.7 2 20.9V3.09996C2 2.29996 2.8 1.79996 3.5 2.09996L16.9 8.79996Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16.9001 15.2L4.1001 21.6L13.7001 12L16.9001 15.2Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M13.7001 11.9999L4.1001 2.3999" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M21.3995 12.95L18.6195 14.34C18.4295 14.44 18.1995 14.4 18.0395 14.25L16.1695 12.38C15.9695 12.18 15.9695 11.87 16.1695 11.67L18.0695 9.77002C18.2195 9.62002 18.4595 9.58002 18.6495 9.68002L21.3995 11.06C22.1895 11.44 22.1895 12.56 21.3995 12.95Z" fill="{color}"/>
<path d="M16.3009 8.49143C16.6109 8.64143 16.6709 9.05145 16.4309 9.29145L14.7609 10.9614L14.0509 11.6715C13.8509 11.8715 13.5409 11.8715 13.3409 11.6715L6.20095 4.53144C5.80095 4.13144 6.27095 3.48145 6.78095 3.73145L16.3009 8.49143Z" fill="{color}"/>
<path d="M2 20.1491V3.47911C2 3.03911 2.53 2.80909 2.85 3.11909L11.62 11.6291C11.83 11.8291 11.82 12.1591 11.61 12.3591L2.84 20.5191C2.52 20.8191 2 20.5891 2 20.1491Z" fill="{color}"/>
<path d="M16.2706 15.5187L6.88056 20.2188C6.37056 20.4688 5.90056 19.8188 6.30056 19.4188L13.3506 12.3688C13.5506 12.1688 13.8606 12.1688 14.0606 12.3688L16.4106 14.7188C16.6406 14.9588 16.5706 15.3687 16.2706 15.5187Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M21.3995 12.9501L16.8795 15.2101L13.6895 12.0201L16.9095 8.80005L21.3995 11.05C22.1895 11.44 22.1895 12.5601 21.3995 12.9501Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 9.06001V3.07002C2 2.27002 2.83 1.76 3.55 2.11L16.92 8.8L13.7 12.02L4.12 21.6L3.54 21.89C2.83 22.24 2 21.73 2 20.93V13.57" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16.8891 15.21L4.11914 21.6L13.6991 12.02L16.8891 15.21Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M13.6998 12.0199L4.08984 2.40991" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16.9206 15.24L16.8906 15.21" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M28.532 17.266l-6.013 3.013-4.253-4.253 4.293-4.293 5.973 3c1.053 0.52 1.053 2.013 0 2.533z"></path>
<path fill="{color}" d="M22.559 11.733l-4.293 4.293-12.893-12.893 17.187 8.6z"></path>
<path fill="{color}" opacity="0.4" d="M18.267 16.027l-12.773 12.773-0.76 0.387c-0.96 0.467-2.067-0.213-2.067-1.28v-23.813c0-1.067 1.107-1.747 2.067-1.28l0.64 0.32 12.893 12.893z"></path>
<path fill="{color}" d="M22.519 20.28l-17.027 8.52 12.773-12.773 4.253 4.253z"></path>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.8896 15.9601C16.6996 15.9601 16.4996 15.8801 16.3596 15.7401L13.1696 12.5501C12.8796 12.2601 12.8796 11.7801 13.1696 11.4901L16.3896 8.27011C16.6196 8.04011 16.9696 7.99013 17.2596 8.13013L21.7496 10.3801C22.3696 10.6801 22.7596 11.3001 22.7596 12.0001C22.7596 12.7001 22.3696 13.3201 21.7496 13.6201L17.2396 15.8801C17.1196 15.9301 16.9996 15.9601 16.8896 15.9601ZM14.7596 12.0201L17.0296 14.2901L21.0596 12.2701C21.0596 12.2701 21.0596 12.2701 21.0696 12.2701C21.2196 12.2001 21.2396 12.0701 21.2396 12.0001C21.2396 11.9301 21.2196 11.8001 21.0696 11.7301L17.0596 9.72012L14.7596 12.0201Z" fill="{color}"/>
<path d="M3.07 22.75C2.74 22.75 2.4 22.66 2.11 22.47C1.57 22.14 1.25 21.56 1.25 20.92V3.06002C1.25 2.43002 1.57 1.85003 2.11 1.51003C2.65 1.18003 3.31 1.14002 3.88 1.43002L17.25 8.12002C17.47 8.23002 17.62 8.43004 17.65 8.67004C17.68 8.91004 17.61 9.15003 17.44 9.32003L4.64 22.12C4.58 22.18 4.52 22.22 4.44 22.26L3.86 22.55C3.62 22.69 3.34 22.75 3.07 22.75ZM3.07 2.75002C3 2.75002 2.94 2.78001 2.9 2.80001C2.84 2.83001 2.75 2.92003 2.75 3.07003V20.93C2.75 21.09 2.84 21.17 2.9 21.2C2.96 21.24 3.07 21.28 3.22 21.21L3.68 20.98L15.65 9.01003L3.21 2.79003C3.16 2.76003 3.11 2.75002 3.07 2.75002Z" fill="{color}"/>
<path d="M4.11999 22.35C3.88999 22.35 3.65999 22.24 3.50999 22.04C3.28999 21.74 3.32999 21.33 3.58999 21.07L13.17 11.49C13.31 11.35 13.5 11.27 13.7 11.27C13.9 11.27 14.09 11.35 14.23 11.49L17.42 14.68C17.59 14.85 17.67 15.09 17.63 15.33C17.59 15.57 17.44 15.77 17.23 15.88L4.46999 22.27C4.34999 22.32 4.23999 22.35 4.11999 22.35ZM13.7 13.08L7.92999 18.85L15.62 15L13.7 13.08Z" fill="{color}"/>
<path d="M13.7003 12.7701C13.5103 12.7701 13.3203 12.7001 13.1703 12.5501L3.56027 2.9401C3.27027 2.6501 3.27027 2.1701 3.56027 1.8801C3.85027 1.5901 4.33027 1.5901 4.62027 1.8801L14.2303 11.4901C14.5203 11.7801 14.5203 12.2601 14.2303 12.5501C14.0903 12.7001 13.8903 12.7701 13.7003 12.7701Z" fill="{color}"/>
<path d="M16.8998 15.9799C16.7198 15.9799 16.5298 15.9099 16.3898 15.7599L16.3598 15.7299C16.0698 15.4399 16.0698 14.9599 16.3698 14.6699C16.6698 14.3799 17.1398 14.3799 17.4298 14.6799C17.7198 14.9699 17.7298 15.4699 17.4398 15.7599C17.2798 15.9099 17.0898 15.9799 16.8998 15.9799Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.92 8.80024L13.7 12.0202L4.12 21.6003L3.54 21.8903C2.83 22.2403 2 21.7303 2 20.9303V3.07026C2 2.27026 2.83 1.76024 3.55 2.11024L16.92 8.80024Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<g opacity="0.4">
<path d="M21.3995 12.9503L16.8795 15.2103L13.6895 12.0203L16.9095 8.80029L21.3995 11.0503C22.1895 11.4403 22.1895 12.5603 21.3995 12.9503Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16.8901 15.21L4.12012 21.6L13.7001 12.02L16.8901 15.21Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M13.6998 12.0201L4.08984 2.41016" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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