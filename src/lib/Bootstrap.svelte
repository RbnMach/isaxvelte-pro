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
<path d="M17 3H7C5.3 3 4 4.3 4 6V6.8C4 7.6 3.9 8.3 3.6 9.1C3.3 10.2 2.2 11 1 11V13C2.2 13 3.3 13.8 3.6 14.9C3.9 15.6 4 16.4 4 17.2V18C4 19.7 5.3 21 7 21H17C18.7 21 20 19.7 20 18V17.2C20 16.4 20.1 15.7 20.4 14.9C20.8 13.8 21.8 13 23 13V11C21.8 11 20.7 10.2 20.4 9.1C20.1 8.4 20 7.6 20 6.8V6C20 4.3 18.7 3 17 3Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
<path d="M9.7998 12H12.6998C13.8998 12 14.7998 12.9 14.7998 14.1C14.7998 15.3 13.8998 16.2 12.6998 16.2H9.7998V7.80005H12.6998C13.8998 7.80005 14.7998 8.70005 14.7998 9.90005C14.7998 11.1 13.8998 12 12.6998 12H9.7998Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12.67 12.75H10.5V15.42H12.67C13.41 15.42 14 14.82 14 14.09C14 13.36 13.4 12.75 12.67 12.75Z" fill="{color}"/>
<path d="M12.67 8.57812H10.5V11.2481H12.67C13.41 11.2481 14 10.6482 14 9.91815C14 9.18815 13.4 8.57812 12.67 8.57812Z" fill="{color}"/>
<path d="M23 11C21.81 11 20.75 10.24 20.37 9.10001C20.13 8.37001 20 7.59999 20 6.82999V6C20 4.34 18.66 3 17 3H7C5.34 3 4 4.34 4 6V6.84C4 7.61 3.88 8.36999 3.63 9.10999C3.25 10.24 2.19 11.01 1 11.01V13.01C2.19 13.01 3.25 13.77 3.63 14.91C3.87 15.64 4 16.41 4 17.17V18C4 19.66 5.34 21 7 21H17C18.66 21 20 19.66 20 18V17.16C20 16.39 20.12 15.63 20.37 14.9C20.75 13.77 21.81 13 23 13V11ZM15.5 14.08C15.5 15.64 14.23 16.91 12.67 16.91H9.75C9.34 16.91 9 16.57 9 16.16V7.82999C9 7.41999 9.34 7.07999 9.75 7.07999H12.67C14.23 7.07999 15.5 8.35 15.5 9.91C15.5 10.73 15.15 11.48 14.58 11.99C15.15 12.52 15.5 13.26 15.5 14.08Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M7 3C5.34 3 4 4.34 4 6V6.84C4 7.61 3.88 8.37001 3.63 9.10001C3.25 10.23 2.19 11 1 11V13C2.19 13 3.25 13.76 3.63 14.9C3.87 15.63 4 16.4 4 17.16V18C4 19.66 5.34 21 7 21H17C18.66 21 20 19.66 20 18V17.16C20 16.39 20.12 15.63 20.37 14.9C20.75 13.77 21.81 13 23 13V11C21.81 11 20.75 10.24 20.37 9.10001C20.13 8.37001 20 7.6 20 6.84V6C20 4.34 18.66 3 17 3H12.25" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9.75 12.0001H12.67C13.82 12.0001 14.75 12.9301 14.75 14.0801C14.75 15.2301 13.82 16.1601 12.67 16.1601H9.75V7.83008H12.67C13.82 7.83008 14.75 8.7601 14.75 9.9101C14.75 11.0601 13.82 11.9901 12.67 11.9901H9.75" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M22.667 4h-13.333c-2.213 0-4 1.787-4 4v1.12c0 1.027-0.16 2.040-0.493 3.013-0.507 1.507-1.92 2.533-3.507 2.533v2.667c1.587 0 3 1.013 3.507 2.533 0.32 0.973 0.493 2 0.493 3.013v1.12c0 2.213 1.787 4 4 4h13.333c2.213 0 4-1.787 4-4v-1.12c0-1.027 0.16-2.040 0.493-3.013 0.507-1.507 1.92-2.533 3.507-2.533v-2.667c-1.587 0-3-1.013-3.507-2.533-0.32-0.973-0.493-2-0.493-3.013v-1.12c0-2.213-1.787-4-4-4z"></path>
<path fill="{color}" d="M16.893 22.56h-3.893c-0.547 0-1-0.453-1-1v-11.107c0-0.547 0.453-1 1-1h3.893c2.080 0 3.773 1.693 3.773 3.773 0 1.093-0.467 2.093-1.227 2.773 0.747 0.693 1.227 1.68 1.227 2.773 0 2.093-1.693 3.787-3.773 3.787zM14 20.56h2.893c0.987 0 1.773-0.8 1.773-1.773s-0.8-1.773-1.773-1.773h-2.893v3.547zM14 15h2.893c0.987 0 1.773-0.8 1.773-1.773s-0.8-1.773-1.773-1.773h-2.893v3.547z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M17 21.75H7C4.93 21.75 3.25 20.07 3.25 18V17.16C3.25 16.47 3.13998 15.79 2.91998 15.13C2.63998 14.3 1.87 13.75 1 13.75C0.59 13.75 0.25 13.41 0.25 13V11C0.25 10.59 0.59 10.25 1 10.25C1.87 10.25 2.64998 9.69 2.91998 8.87C3.13998 8.21 3.25 7.53 3.25 6.84V6C3.25 3.93 4.93 2.25 7 2.25H17C19.07 2.25 20.75 3.93 20.75 6V6.84C20.75 7.53 20.86 8.21 21.08 8.87C21.36 9.7 22.13 10.25 23 10.25C23.41 10.25 23.75 10.59 23.75 11V13C23.75 13.41 23.41 13.75 23 13.75C22.13 13.75 21.35 14.31 21.08 15.13C20.86 15.79 20.75 16.47 20.75 17.16V18C20.75 20.07 19.07 21.75 17 21.75ZM1.75 12.33C2.95 12.59 3.94003 13.46 4.34003 14.66C4.61003 15.47 4.75 16.31 4.75 17.16V18C4.75 19.24 5.76 20.25 7 20.25H17C18.24 20.25 19.25 19.24 19.25 18V17.16C19.25 16.31 19.39 15.47 19.66 14.66C20.06 13.46 21.06 12.59 22.25 12.33V11.67C21.05 11.41 20.06 10.54 19.66 9.34C19.39 8.53 19.25 7.69 19.25 6.84V6C19.25 4.76 18.24 3.75 17 3.75H7C5.76 3.75 4.75 4.76 4.75 6V6.84C4.75 7.69 4.61003 8.53 4.34003 9.34C3.94003 10.54 2.94 11.41 1.75 11.67V12.33Z" fill="{color}"/>
<path d="M12.67 16.9199H9.75C9.34 16.9199 9 16.5799 9 16.1699V7.83984C9 7.42984 9.34 7.08984 9.75 7.08984H12.67C14.23 7.08984 15.5 8.35986 15.5 9.91986C15.5 10.7399 15.15 11.4898 14.58 11.9998C15.14 12.5198 15.5 13.2598 15.5 14.0798C15.5 15.6498 14.23 16.9199 12.67 16.9199ZM10.5 15.4199H12.67C13.41 15.4199 14 14.8198 14 14.0898C14 13.3598 13.4 12.7599 12.67 12.7599H10.5V15.4199ZM10.5 11.2498H12.67C13.41 11.2498 14 10.6499 14 9.91986C14 9.18986 13.4 8.58984 12.67 8.58984H10.5V11.2498Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M17 3H7C5.34 3 4 4.34 4 6V6.84C4 7.61 3.88 8.37001 3.63 9.10001C3.25 10.23 2.19 11 1 11V13C2.19 13 3.25 13.76 3.63 14.9C3.87 15.63 4 16.4 4 17.16V18C4 19.66 5.34 21 7 21H17C18.66 21 20 19.66 20 18V17.16C20 16.39 20.12 15.63 20.37 14.9C20.75 13.77 21.81 13 23 13V11C21.81 11 20.75 10.24 20.37 9.10001C20.13 8.37001 20 7.6 20 6.84V6C20 4.34 18.66 3 17 3Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
<path opacity="0.4" d="M9.75 12.0001H12.67C13.82 12.0001 14.75 12.9301 14.75 14.0801C14.75 15.2301 13.82 16.1601 12.67 16.1601H9.75V7.83008H12.67C13.82 7.83008 14.75 8.7601 14.75 9.9101C14.75 11.0601 13.82 11.9901 12.67 11.9901H9.75" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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