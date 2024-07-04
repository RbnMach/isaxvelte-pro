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
<path d="M8 2.8C9.2 2.3 10.6 2 12 2C17.5 2 22 6.5 22 12C22 17.5 17.5 22 12 22C6.5 22 2 17.5 2 12C2 10.6 2.3 9.2 2.8 8" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16.0001 16.2V12C16.0001 9.70005 14.1001 7.80005 11.8001 7.80005C9.5001 7.80005 7.6001 9.70005 7.6001 12C7.6001 14.3 9.5001 16.2 11.8001 16.2H16.0001Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5 6.5C5.82843 6.5 6.5 5.82843 6.5 5C6.5 4.17157 5.82843 3.5 5 3.5C4.17157 3.5 3.5 4.17157 3.5 5C3.5 5.82843 4.17157 6.5 5 6.5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 10.51 1.55001 9.08 2.14001 7.72C2.31001 7.34 2.75 7.17 3.13 7.33C3.51 7.5 3.68002 7.94001 3.52002 8.32001C3.02002 9.48001 2.76001 10.72 2.76001 12C2.76001 17.1 6.91001 21.25 12.01 21.25C17.11 21.25 21.26 17.1 21.26 12C21.26 6.9 17.11 2.75 12.01 2.75C10.72 2.75 9.45998 3.01 8.28998 3.53C7.91998 3.7 7.46999 3.52999 7.29999 3.14999C7.12999 2.76999 7.29999 2.33 7.67999 2.16C9.04999 1.56 10.5 1.25 12.01 1.25C17.94 1.25 22.76 6.07 22.76 12C22.76 17.93 17.93 22.75 12 22.75Z" fill="{color}"/>
<path d="M16 15.25V12C16 9.65 14.1 7.75 11.75 7.75C9.4 7.75 7.5 9.65 7.5 12C7.5 14.35 9.4 16.25 11.75 16.25H15C15.55 16.25 16 15.8 16 15.25Z" fill="{color}"/>
<path d="M4.99915 6.8811C6.03744 6.8811 6.87915 6.03939 6.87915 5.0011C6.87915 3.9628 6.03744 3.12109 4.99915 3.12109C3.96085 3.12109 3.11914 3.9628 3.11914 5.0011C3.11914 6.03939 3.96085 6.8811 4.99915 6.8811Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.3 21.03C15 21.65 13.54 22 12 22C6.48 22 2 17.52 2 12C2 10.59 2.29001 9.24002 2.82001 8.02002" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7.9707 2.84C9.2007 2.3 10.5607 2 12.0007 2C17.5207 2 22.0007 6.48 22.0007 12C22.0007 14.29 21.2307 16.4 19.9407 18.08" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16 16.25V12C16 9.65 14.1 7.75 11.75 7.75C9.4 7.75 7.5 9.65 7.5 12C7.5 14.35 9.4 16.25 11.75 16.25H16Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5 6.5C5.82843 6.5 6.5 5.82843 6.5 5C6.5 4.17157 5.82843 3.5 5 3.5C4.17157 3.5 3.5 4.17157 3.5 5C3.5 5.82843 4.17157 6.5 5 6.5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 30.333c-7.907 0-14.333-6.427-14.333-14.333 0-1.987 0.4-3.893 1.187-5.707 0.227-0.507 0.813-0.733 1.32-0.52 0.507 0.227 0.733 0.813 0.52 1.32-0.667 1.547-1.013 3.2-1.013 4.907 0 6.8 5.533 12.333 12.333 12.333s12.333-5.533 12.333-12.333c0-6.8-5.547-12.333-12.347-12.333-1.72 0-3.4 0.347-4.96 1.040-0.493 0.227-1.093 0-1.32-0.507s0-1.093 0.507-1.32c1.827-0.8 3.76-1.213 5.773-1.213 7.907 0 14.333 6.427 14.333 14.333s-6.427 14.333-14.333 14.333z"></path>
<path fill="{color}" d="M21.333 20.333v-4.333c0-3.133-2.533-5.667-5.667-5.667s-5.667 2.533-5.667 5.667c0 3.133 2.533 5.667 5.667 5.667h4.333c0.733 0 1.333-0.6 1.333-1.333z"></path>
<path fill="{color}" d="M6.666 9.174c1.384 0 2.507-1.122 2.507-2.507s-1.122-2.507-2.507-2.507c-1.384 0-2.507 1.122-2.507 2.507s1.122 2.507 2.507 2.507z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 10.51 1.55001 9.08 2.14001 7.72C2.31001 7.34 2.75 7.17 3.13 7.33C3.51 7.5 3.68002 7.94001 3.52002 8.32001C3.02002 9.48001 2.76001 10.72 2.76001 12C2.76001 17.1 6.91001 21.25 12.01 21.25C17.11 21.25 21.26 17.1 21.26 12C21.26 6.9 17.11 2.75 12.01 2.75C10.72 2.75 9.45998 3.01 8.28998 3.53C7.91998 3.7 7.46999 3.52999 7.29999 3.14999C7.12999 2.76999 7.29999 2.33 7.67999 2.16C9.04999 1.56 10.5 1.25 12.01 1.25C17.94 1.25 22.76 6.07 22.76 12C22.76 17.93 17.93 22.75 12 22.75Z" fill="{color}"/>
<path d="M16 17H11.75C8.99 17 6.75 14.76 6.75 12C6.75 9.24 8.99 7 11.75 7C14.51 7 16.75 9.24 16.75 12V16.25C16.75 16.66 16.41 17 16 17ZM11.75 8.5C9.82 8.5 8.25 10.07 8.25 12C8.25 13.93 9.82 15.5 11.75 15.5H15.25V12C15.25 10.07 13.68 8.5 11.75 8.5Z" fill="{color}"/>
<path d="M5 7.25C3.76 7.25 2.75 6.24 2.75 5C2.75 3.76 3.76 2.75 5 2.75C6.24 2.75 7.25 3.76 7.25 5C7.25 6.24 6.24 7.25 5 7.25ZM5 4.25C4.59 4.25 4.25 4.59 4.25 5C4.25 5.41 4.59 5.75 5 5.75C5.41 5.75 5.75 5.41 5.75 5C5.75 4.59 5.41 4.25 5 4.25Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M7.96997 2.84C9.19997 2.3 10.56 2 12 2C17.52 2 22 6.48 22 12C22 17.52 17.52 22 12 22C6.48 22 2 17.52 2 12C2 10.59 2.29001 9.24 2.82001 8.02" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M16 16.25V12C16 9.65 14.1 7.75 11.75 7.75C9.4 7.75 7.5 9.65 7.5 12C7.5 14.35 9.4 16.25 11.75 16.25H16Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M5 6.5C5.82843 6.5 6.5 5.82843 6.5 5C6.5 4.17157 5.82843 3.5 5 3.5C4.17157 3.5 3.5 4.17157 3.5 5C3.5 5.82843 4.17157 6.5 5 6.5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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