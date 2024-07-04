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
<path d="M15 22H9C4 22 2 20 2 15V9C2 4 4 2 9 2H15C20 2 22 4 22 9V15C22 20 20 22 15 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17.9999 8.5V15.6H16.1999C15.1999 15.6 14.3999 14.8 14.3999 13.8C14.3999 12.8 15.1999 12 16.1999 12H17.9999" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6 8.5L11.7 15.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.7 8.5L6 15.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15.1699 13.7719C15.1699 14.3319 15.6299 14.7919 16.1899 14.7919H17.2099V12.7619H16.1899C15.6299 12.7519 15.1699 13.2119 15.1699 13.7719Z" fill="{color}"/>
<path d="M16.1898 2H7.81978C4.17978 2 2.00977 4.17 2.00977 7.81V16.18C2.00977 19.82 4.17978 21.99 7.81978 21.99H16.1898C19.8298 21.99 21.9998 19.82 21.9998 16.18V7.81C21.9998 4.17 19.8298 2 16.1898 2ZM12.2798 15.06C12.5398 15.38 12.4898 15.86 12.1598 16.11C12.0198 16.22 11.8598 16.27 11.6898 16.27C11.4698 16.27 11.2498 16.17 11.0998 15.99L8.85977 13.19L6.61977 15.99C6.46977 16.17 6.24977 16.27 6.02977 16.27C5.86977 16.27 5.69977 16.22 5.55977 16.11C5.23977 15.85 5.17977 15.38 5.43977 15.06L7.88977 12L5.43977 8.94C5.17977 8.62 5.22977 8.14001 5.55977 7.89001C5.87977 7.63001 6.35977 7.68001 6.60977 8.01001L8.84978 10.81L11.0898 8.01001C11.3498 7.69001 11.8198 7.63001 12.1398 7.89001C12.4598 8.15001 12.5198 8.62 12.2598 8.94L9.80977 12L12.2798 15.06ZM18.7098 15.53C18.7098 15.94 18.3698 16.28 17.9598 16.28H16.1898C14.7998 16.28 13.6698 15.15 13.6698 13.76C13.6698 12.37 14.7998 11.24 16.1898 11.24H17.2098V8.45999C17.2098 8.04999 17.5498 7.70999 17.9598 7.70999C18.3698 7.70999 18.7098 8.04999 18.7098 8.45999V15.53Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M17.9599 8.46997V15.53H16.1899C15.2099 15.53 14.4199 14.74 14.4199 13.76C14.4199 12.78 15.2099 11.99 16.1899 11.99H17.9599" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6.03906 8.46997L11.6891 15.53" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.6891 8.46997L6.03906 15.53" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 12.83V15C2 20 4 22 9 22H15C20 22 22 20 22 15V9C22 4 20 2 15 2H9C4 2 2 4 2 9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M21.586 2.667h-11.16c-4.853 0-7.747 2.893-7.747 7.747v11.16c0 4.853 2.893 7.747 7.747 7.747h11.16c4.853 0 7.747-2.893 7.747-7.747v-11.16c0-4.853-2.893-7.747-7.747-7.747z"></path>
<path fill="{color}" d="M23.947 10.293c-0.547 0-1 0.453-1 1v3.707h-1.36c-1.853 0-3.36 1.507-3.36 3.36s1.507 3.36 3.36 3.36h2.36c0.547 0 1-0.453 1-1v-9.413c0-0.573-0.453-1.013-1-1.013zM22.947 19.706h-1.36c-0.747 0-1.36-0.613-1.36-1.36s0.613-1.36 1.36-1.36h1.36v2.72z"></path>
<path fill="{color}" d="M16.214 10.506c-0.427-0.347-1.067-0.28-1.4 0.16l-2.987 3.733-2.987-3.733c-0.347-0.427-0.973-0.507-1.4-0.16s-0.507 0.973-0.16 1.4l3.267 4.080-3.267 4.080c-0.347 0.427-0.28 1.067 0.16 1.4 0.187 0.147 0.4 0.213 0.627 0.213 0.293 0 0.587-0.133 0.787-0.373l2.987-3.733 2.987 3.733c0.2 0.24 0.493 0.373 0.787 0.373 0.213 0 0.44-0.067 0.627-0.213 0.427-0.347 0.507-0.973 0.16-1.4l-3.267-4.080 3.267-4.080c0.32-0.427 0.253-1.053-0.187-1.4z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15 22.75H9C3.57 22.75 1.25 20.43 1.25 15V9C1.25 3.57 3.57 1.25 9 1.25H15C20.43 1.25 22.75 3.57 22.75 9V15C22.75 20.43 20.43 22.75 15 22.75ZM9 2.75C4.39 2.75 2.75 4.39 2.75 9V15C2.75 19.61 4.39 21.25 9 21.25H15C19.61 21.25 21.25 19.61 21.25 15V9C21.25 4.39 19.61 2.75 15 2.75H9Z" fill="{color}"/>
<path d="M17.9599 16.28H16.1899C14.7999 16.28 13.6699 15.15 13.6699 13.76C13.6699 12.37 14.7999 11.24 16.1899 11.24H17.2099V8.45996C17.2099 8.04996 17.5499 7.70996 17.9599 7.70996C18.3699 7.70996 18.7099 8.04996 18.7099 8.45996V15.52C18.7099 15.95 18.3699 16.28 17.9599 16.28ZM16.1899 12.75C15.6299 12.75 15.1699 13.21 15.1699 13.77C15.1699 14.33 15.6299 14.79 16.1899 14.79H17.2099V12.76H16.1899V12.75Z" fill="{color}"/>
<path d="M11.69 16.2799C11.47 16.2799 11.25 16.1799 11.1 15.9999L5.45001 8.93994C5.19001 8.61994 5.24002 8.13995 5.57002 7.88995C5.89002 7.62995 6.37 7.67995 6.62 8.00995L12.27 15.0699C12.53 15.3899 12.48 15.8699 12.15 16.1199C12.02 16.2299 11.86 16.2799 11.69 16.2799Z" fill="{color}"/>
<path d="M6.03981 16.2802C5.87981 16.2802 5.70983 16.2302 5.56983 16.1202C5.24983 15.8602 5.18981 15.3902 5.44981 15.0702L11.0998 8.01025C11.3598 7.69025 11.8298 7.63025 12.1498 7.89025C12.4698 8.15025 12.5298 8.62024 12.2698 8.94024L6.61981 16.0002C6.47981 16.1802 6.25981 16.2802 6.03981 16.2802Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15 22H9C4 22 2 20 2 15V9C2 4 4 2 9 2H15C20 2 22 4 22 9V15C22 20 20 22 15 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M17.9599 8.47021V15.5302H16.1899C15.2099 15.5302 14.4199 14.7402 14.4199 13.7602C14.4199 12.7802 15.2099 11.9902 16.1899 11.9902H17.9599" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<g opacity="0.4">
<path d="M6.04004 8.46973L11.69 15.5297" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.69 8.46973L6.04004 15.5297" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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