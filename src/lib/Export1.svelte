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
<path d="M9.31995 6.49994L11.8799 3.93994L14.4399 6.49994" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.88 14.18V4.01001" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 12C4 16.42 7 20 12 20C17 20 20 16.42 20 12" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M21.14 9.89844H12.75V15.3784C12.75 15.7884 12.41 16.1284 12 16.1284C11.59 16.1284 11.25 15.7884 11.25 15.3784V9.89844H2.86C2.38 9.89844 2 10.2784 2 10.7584C2 16.6484 6.11 20.7584 12 20.7584C17.89 20.7584 22 16.6484 22 10.7584C22 10.2784 21.62 9.89844 21.14 9.89844Z" fill="{color}"/>
<path d="M12.7484 5.79969L14.3084 7.35969C14.5984 7.64969 15.0784 7.64969 15.3684 7.35969C15.6584 7.06969 15.6584 6.58969 15.3684 6.29969L12.5184 3.45969C12.2284 3.16969 11.7484 3.16969 11.4584 3.45969L8.61844 6.30969C8.47844 6.45969 8.39844 6.64969 8.39844 6.83969C8.39844 7.02969 8.46844 7.21969 8.61844 7.36969C8.90844 7.65969 9.38844 7.65969 9.67844 7.36969L11.2384 5.80969V9.89969H12.7384V5.79969H12.7484Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M17.52 18.01C16.16 19.25 14.29 20 12 20C7 20 4 16.42 4 12" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M19.9998 12C19.9998 13.05 19.8298 14.05 19.5098 14.97" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9.43945 6.46991L11.9995 3.90991L14.5595 6.46991" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 9.14998V3.97998" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 14.1499V12.1899" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M22 10.7599C22 10.2899 21.62 9.8999 21.14 9.8999H2.86C2.38 9.8999 2 10.2799 2 10.7599C2 16.6499 6.11 20.7599 12 20.7599C17.89 20.7599 22 16.6399 22 10.7599Z" fill="{color}"/>
<path d="M12.5304 3.45992L15.3804 6.29992C15.6704 6.58992 15.6704 7.06992 15.3804 7.35992C15.0904 7.64992 14.6104 7.64992 14.3204 7.35992L12.7504 5.79992V15.3699C12.7504 15.7799 12.4104 16.1199 12.0004 16.1199C11.5904 16.1199 11.2504 15.7799 11.2504 15.3699V5.79992L9.69039 7.36992C9.40039 7.65992 8.92039 7.65992 8.63039 7.36992C8.48039 7.21992 8.40039 7.02992 8.40039 6.83992C8.40039 6.64992 8.47039 6.45992 8.62039 6.30992L11.4704 3.46992C11.7604 3.16992 12.2404 3.16992 12.5304 3.45992Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M14.4398 7.24988C14.2498 7.24988 14.0598 7.17988 13.9098 7.02988L11.8798 4.99988L9.84977 7.02988C9.55977 7.31988 9.07977 7.31988 8.78977 7.02988C8.49977 6.73988 8.49977 6.25988 8.78977 5.96988L11.3498 3.40988C11.6398 3.11988 12.1198 3.11988 12.4098 3.40988L14.9698 5.96988C15.2598 6.25988 15.2598 6.73988 14.9698 7.02988C14.8198 7.17988 14.6298 7.24988 14.4398 7.24988Z" fill="{color}"/>
<path d="M11.8809 14.93C11.4709 14.93 11.1309 14.59 11.1309 14.18V4.01001C11.1309 3.60001 11.4709 3.26001 11.8809 3.26001C12.2909 3.26001 12.6309 3.60001 12.6309 4.01001V14.18C12.6309 14.6 12.2909 14.93 11.8809 14.93Z" fill="{color}"/>
<path d="M12 20.75C6.85 20.75 3.25 17.15 3.25 12C3.25 11.59 3.59 11.25 4 11.25C4.41 11.25 4.75 11.59 4.75 12C4.75 16.27 7.73 19.25 12 19.25C16.27 19.25 19.25 16.27 19.25 12C19.25 11.59 19.59 11.25 20 11.25C20.41 11.25 20.75 11.59 20.75 12C20.75 17.15 17.15 20.75 12 20.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<g opacity="0.4">
<path d="M9.32031 6.50043L11.8803 3.94043L14.4403 6.50043" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.8809 14.1798V4.00977" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</g>
<path d="M4 12C4 16.42 7 20 12 20C17 20 20 16.42 20 12" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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