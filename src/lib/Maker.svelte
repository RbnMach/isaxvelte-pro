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
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6.6001 14.5V9.5L10.8001 12V14.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17.4002 14.5V9.5L13.2002 12V14.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM11.5 14.5C11.5 14.91 11.16 15.25 10.75 15.25C10.34 15.25 10 14.91 10 14.5V12.42L7.33002 10.82V14.5C7.33002 14.91 6.99002 15.25 6.58002 15.25C6.17002 15.25 5.83002 14.91 5.83002 14.5V9.5C5.83002 9.23 5.98002 8.98 6.21002 8.85C6.44002 8.72 6.73002 8.72 6.96002 8.86L11.13 11.36C11.36 11.5 11.49 11.74 11.49 12V14.5H11.5ZM18.17 14.5C18.17 14.91 17.83 15.25 17.42 15.25C17.01 15.25 16.67 14.91 16.67 14.5V10.82L14 12.42V14.5C14 14.91 13.66 15.25 13.25 15.25C12.84 15.25 12.5 14.91 12.5 14.5V12C12.5 11.74 12.64 11.49 12.86 11.36L17.03 8.86C17.26 8.72 17.55 8.72 17.78 8.85C18.02 8.98 18.16 9.23 18.16 9.5V14.5H18.17Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M6.58008 14.5V9.5L10.7501 12V14.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17.42 14.5V9.5L13.25 12V14.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.19997 2.3 7.96997 2.85" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M14.333 20.334c-0.547 0-1-0.453-1-1v-2.773l-3.56-2.133v4.907c0 0.547-0.453 1-1 1s-1-0.453-1-1v-6.667c0-0.36 0.2-0.693 0.507-0.867s0.693-0.173 1 0.013l5.56 3.333c0.307 0.187 0.48 0.507 0.48 0.853v3.333c0.013 0.547-0.44 1-0.987 1z"></path>
<path fill="{color}" d="M23.227 20.334c-0.547 0-1-0.453-1-1v-4.907l-3.56 2.133v2.773c0 0.547-0.453 1-1 1s-1-0.453-1-1v-3.333c0-0.347 0.187-0.68 0.48-0.853l5.56-3.333c0.307-0.187 0.693-0.187 1-0.013 0.32 0.173 0.507 0.507 0.507 0.867v6.667c0.013 0.547-0.44 1-0.987 1z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
<path d="M10.7501 15.2502C10.3401 15.2502 10.0001 14.9102 10.0001 14.5002V12.4202L7.33008 10.8202V14.5002C7.33008 14.9102 6.99008 15.2502 6.58008 15.2502C6.17008 15.2502 5.83008 14.9102 5.83008 14.5002V9.50019C5.83008 9.23019 5.98008 8.98019 6.21008 8.85019C6.44008 8.72019 6.73008 8.72019 6.96008 8.86019L11.1301 11.3602C11.3601 11.5002 11.4901 11.7402 11.4901 12.0002V14.5002C11.5001 14.9102 11.1601 15.2502 10.7501 15.2502Z" fill="{color}"/>
<path d="M17.42 15.2502C17.01 15.2502 16.67 14.9102 16.67 14.5002V10.8202L14 12.4202V14.5002C14 14.9102 13.66 15.2502 13.25 15.2502C12.84 15.2502 12.5 14.9102 12.5 14.5002V12.0002C12.5 11.7402 12.64 11.4902 12.86 11.3602L17.03 8.86019C17.26 8.72019 17.55 8.72019 17.78 8.85019C18.02 8.98019 18.16 9.23019 18.16 9.50019V14.5002C18.17 14.9102 17.83 15.2502 17.42 15.2502Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M6.58008 14.5V9.5L10.7501 12V14.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M17.42 14.5V9.5L13.25 12V14.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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