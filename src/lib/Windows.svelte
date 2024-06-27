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
<path fill-rule="evenodd" clip-rule="evenodd" d="M22 2L12 4V11H22V2Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path fill-rule="evenodd" clip-rule="evenodd" d="M22 22L12 20V13H22V22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path fill-rule="evenodd" clip-rule="evenodd" d="M10 4.30005L2 6.00005V11H10V4.30005Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path fill-rule="evenodd" clip-rule="evenodd" d="M10 19.7L2 18V13H10V19.7Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path fill-rule="evenodd" clip-rule="evenodd" d="M20.8 2.24144L12.8 3.84145C12.33 3.93145 12 4.34146 12 4.82146V10.0015C12 10.5514 12.45 11.0015 13 11.0015H21C21.55 11.0015 22 10.5514 22 10.0015V3.22145C22 2.59145 21.42 2.12144 20.8 2.24144Z" fill="{color}"/>
<path fill-rule="evenodd" clip-rule="evenodd" d="M20.8 21.76L12.8 20.16C12.33 20.07 12 19.66 12 19.18V14C12 13.45 12.45 13 13 13H21C21.55 13 22 13.45 22 14V20.78C22 21.41 21.42 21.88 20.8 21.76Z" fill="{color}"/>
<path fill-rule="evenodd" clip-rule="evenodd" d="M8.78998 4.55959L2.78998 5.82958C2.32998 5.92958 2 6.33959 2 6.80959V9.99959C2 10.5496 2.45 10.9996 3 10.9996H9C9.55 10.9996 10 10.5496 10 9.99959V5.52959C10 4.89959 9.40998 4.41959 8.78998 4.55959Z" fill="{color}"/>
<path fill-rule="evenodd" clip-rule="evenodd" d="M8.78998 19.44L2.78998 18.17C2.32998 18.07 2 17.66 2 17.19V14C2 13.45 2.45 13 3 13H9C9.55 13 10 13.45 10 14V18.47C10 19.1 9.40998 19.58 8.78998 19.44Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M22 6.03V2L12 4V11H22" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path fill-rule="evenodd" clip-rule="evenodd" d="M22 22L12 20V13H22V22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
<path fill-rule="evenodd" clip-rule="evenodd" d="M10 4.30005L2 6.00006V11.0001H10V4.30005Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
<path fill-rule="evenodd" clip-rule="evenodd" d="M10 19.7L2 18V13H10V19.7Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M27.733 2.987l-10.667 2.133c-0.627 0.12-1.067 0.667-1.067 1.307v6.907c0 0.733 0.6 1.333 1.333 1.333h10.667c0.733 0 1.333-0.6 1.333-1.333v-9.040c0-0.84-0.773-1.467-1.6-1.307z"></path>
<path fill="{color}" d="M27.733 29.013l-10.667-2.133c-0.627-0.12-1.067-0.667-1.067-1.307v-6.907c0-0.733 0.6-1.333 1.333-1.333h10.667c0.733 0 1.333 0.6 1.333 1.333v9.040c0 0.84-0.773 1.467-1.6 1.307z"></path>
<path fill="{color}" d="M11.72 6.080l-8 1.707c-0.613 0.133-1.053 0.68-1.053 1.307v4.24c0 0.733 0.6 1.333 1.333 1.333h8c0.733 0 1.333-0.6 1.333-1.333v-5.96c0-0.84-0.787-1.48-1.613-1.293z"></path>
<path fill="{color}" opacity="0.4" d="M11.72 25.92l-8-1.707c-0.613-0.133-1.053-0.68-1.053-1.307v-4.24c0-0.733 0.6-1.333 1.333-1.333h8c0.733 0 1.333 0.6 1.333 1.333v5.96c0 0.84-0.787 1.48-1.613 1.293z"></path>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M22 11.7498H12C11.59 11.7498 11.25 11.4098 11.25 10.9998V3.9998C11.25 3.6398 11.5 3.32981 11.85 3.25981L21.85 1.25981C22.07 1.21981 22.3 1.26981 22.47 1.41981C22.64 1.55981 22.74 1.7798 22.74 1.9998V10.9998C22.75 11.4098 22.41 11.7498 22 11.7498ZM12.75 10.2498H21.25V2.91981L12.75 4.61979V10.2498Z" fill="{color}"/>
<path d="M22 22.75C21.95 22.75 21.9 22.75 21.85 22.74L11.85 20.74C11.5 20.67 11.25 20.36 11.25 20V13C11.25 12.59 11.59 12.25 12 12.25H22C22.41 12.25 22.75 12.59 22.75 13V22C22.75 22.22 22.65 22.44 22.48 22.58C22.34 22.69 22.17 22.75 22 22.75ZM12.75 19.38L21.25 21.08V13.75H12.75V19.38Z" fill="{color}"/>
<path d="M10 11.7501H2C1.59 11.7501 1.25 11.4101 1.25 11.0001V6.00014C1.25 5.65014 1.50003 5.34013 1.84003 5.27013L9.84003 3.57015C10.06 3.52015 10.29 3.58014 10.47 3.72014C10.65 3.86014 10.75 4.08013 10.75 4.30013V11.0001C10.75 11.4101 10.41 11.7501 10 11.7501ZM2.75 10.2501H9.25V5.23015L2.75 6.61013V10.2501Z" fill="{color}"/>
<path d="M10 20.45C9.95 20.45 9.90003 20.44 9.84003 20.43L1.84003 18.73C1.49003 18.66 1.25 18.35 1.25 18V13C1.25 12.59 1.59 12.25 2 12.25H10C10.41 12.25 10.75 12.59 10.75 13V19.7C10.75 19.93 10.65 20.14 10.47 20.28C10.34 20.39 10.17 20.45 10 20.45ZM2.75 17.39L9.25 18.77V13.75H2.75V17.39Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" fill-rule="evenodd" clip-rule="evenodd" d="M22 2L12 4V11H22V2Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
<path fill-rule="evenodd" clip-rule="evenodd" d="M22 22L12 20V13H22V22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
<path fill-rule="evenodd" clip-rule="evenodd" d="M10 4.2998L2 5.99982V10.9998H10V4.2998Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
<path opacity="0.4" fill-rule="evenodd" clip-rule="evenodd" d="M10 19.7L2 18V13H10V19.7Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
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