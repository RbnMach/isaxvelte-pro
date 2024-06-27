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
<path d="M3.5 22H20.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5 3.5L19 17.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5 13.77V3.5H15.27" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M20.5 21.25H3.5C3.09 21.25 2.75 21.59 2.75 22C2.75 22.41 3.09 22.75 3.5 22.75H20.5C20.91 22.75 21.25 22.41 21.25 22C21.25 21.59 20.91 21.25 20.5 21.25Z" fill="{color}"/>
<path d="M5 14.52C5.41 14.52 5.75 14.18 5.75 13.77V5.31L18.47 18.03C18.62 18.18 18.81 18.25 19 18.25C19.19 18.25 19.38 18.18 19.53 18.03C19.82 17.74 19.82 17.26 19.53 16.97L6.81 4.25H15.27C15.68 4.25 16.02 3.91 16.02 3.5C16.02 3.09 15.68 2.75 15.27 2.75H5C4.9 2.75 4.81 2.77 4.71 2.81C4.53 2.88 4.38 3.03 4.31 3.21C4.27 3.31 4.25 3.4 4.25 3.5V13.77C4.25 14.18 4.59 14.52 5 14.52Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <path d="M16.59,15.1l2.41,2.41" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
  <path d="M5.01,3.49l8.37,8.39" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
  <path d="M5,13.76V3.49s10.28.01,10.28.01" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
  <path d="M3.5,22h17" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
</svg>
	{/if}										
	{#if type == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M20.4992 22.8002H3.49922C3.09922 22.8002 2.69922 22.5002 2.69922 22.0002C2.69922 21.5002 2.99922 21.2002 3.49922 21.2002H20.4992C20.8992 21.2002 21.2992 21.5002 21.2992 22.0002C21.2992 22.5002 20.8992 22.8002 20.4992 22.8002Z" fill="{color}"/>
<path d="M18.9984 18.2004C18.7984 18.2004 18.5984 18.1004 18.4984 18.0004L4.49844 4.00039C4.19844 3.70039 4.19844 3.30039 4.49844 3.00039C4.79844 2.70039 5.29844 2.70039 5.59844 3.00039L19.5984 17.0004C19.8984 17.3004 19.8984 17.8004 19.5984 18.1004C19.3984 18.2004 19.1984 18.2004 18.9984 18.2004Z" fill="{color}"/>
<path d="M4.99922 14.5002C4.59922 14.5002 4.19922 14.2002 4.19922 13.7002V3.5002C4.19922 3.1002 4.49922 2.7002 4.99922 2.7002H15.2992C15.6992 2.7002 16.0992 3.0002 16.0992 3.5002C16.0992 4.0002 15.7992 4.3002 15.2992 4.3002H5.79922V13.8002C5.79922 14.2002 5.39922 14.5002 4.99922 14.5002Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M20.5 22.75H3.5C3.09 22.75 2.75 22.41 2.75 22C2.75 21.59 3.09 21.25 3.5 21.25H20.5C20.91 21.25 21.25 21.59 21.25 22C21.25 22.41 20.91 22.75 20.5 22.75Z" fill="{color}"/>
<path d="M18.9995 18.2499C18.8095 18.2499 18.6195 18.1799 18.4695 18.0299L4.46945 4.02994C4.17945 3.73994 4.17945 3.25994 4.46945 2.96994C4.75945 2.67994 5.23945 2.67994 5.52945 2.96994L19.5295 16.9699C19.8195 17.2599 19.8195 17.7399 19.5295 18.0299C19.3795 18.1799 19.1895 18.2499 18.9995 18.2499Z" fill="{color}"/>
<path d="M5 14.52C4.59 14.52 4.25 14.18 4.25 13.77V3.5C4.25 3.09 4.59 2.75 5 2.75H15.27C15.68 2.75 16.02 3.09 16.02 3.5C16.02 3.91 15.68 4.25 15.27 4.25H5.75V13.77C5.75 14.18 5.41 14.52 5 14.52Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M3.5 22H20.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5 3.5L19 17.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5 13.77V3.5H15.27" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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