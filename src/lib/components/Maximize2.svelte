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
<path d="M2 9V6.5C2 4.01 4.01 2 6.5 2H9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15 2H17.5C19.99 2 22 4.01 22 6.5V9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M22 16V17.5C22 19.99 19.99 22 17.5 22H16" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9 22H6.5C4.01 22 2 19.99 2 17.5V15" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.19 2H7.81C4.17 2 2 4.17 2 7.81V16.18C2 19.83 4.17 22 7.81 22H16.18C19.82 22 21.99 19.83 21.99 16.19V7.81C22 4.17 19.83 2 16.19 2ZM10.22 21H7.91C5.2 21 3 18.8 3 16.09V13.78C3 13.37 3.34 13.03 3.75 13.03C4.16 13.03 4.5 13.37 4.5 13.78V16.09C4.5 17.97 6.03 19.5 7.91 19.5H10.22C10.63 19.5 10.97 19.84 10.97 20.25C10.97 20.66 10.64 21 10.22 21ZM10.22 4.5H7.91C6.03 4.5 4.5 6.03 4.5 7.91V10.22C4.5 10.63 4.16 10.97 3.75 10.97C3.34 10.97 3 10.64 3 10.22V7.91C3 5.2 5.2 3 7.91 3H10.22C10.63 3 10.97 3.34 10.97 3.75C10.97 4.16 10.64 4.5 10.22 4.5ZM21 16.09C21 18.8 18.8 21 16.09 21H14.7C14.29 21 13.95 20.66 13.95 20.25C13.95 19.84 14.29 19.5 14.7 19.5H16.09C17.97 19.5 19.5 17.97 19.5 16.09V14.7C19.5 14.29 19.84 13.95 20.25 13.95C20.66 13.95 21 14.29 21 14.7V16.09ZM21 10.22C21 10.63 20.66 10.97 20.25 10.97C19.84 10.97 19.5 10.63 19.5 10.22V7.91C19.5 6.03 17.97 4.5 16.09 4.5H13.78C13.37 4.5 13.03 4.16 13.03 3.75C13.03 3.34 13.36 3 13.78 3H16.09C18.8 3 21 5.2 21 7.91V10.22Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2 9V6.5C2 4.01 4.01 2 6.5 2H9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15 2H17.5C19.99 2 22 4.01 22 6.5V9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M22 16V17.5C22 19.99 19.99 22 17.5 22H16" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9 22H6.5C4.01 22 2 19.99 2 17.5V15" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M16.19 2H7.81C4.17 2 2 4.17 2 7.81V16.18C2 19.83 4.17 22 7.81 22H16.18C19.82 22 21.99 19.83 21.99 16.19V7.81C22 4.17 19.83 2 16.19 2Z" fill="{color}"/>
<path d="M2.75 9.97C2.34 9.97 2 9.64 2 9.22V6.91C2 4.2 4.2 2 6.91 2H9.22C9.63 2 9.97 2.34 9.97 2.75C9.97 3.16 9.64 3.5 9.22 3.5H6.91C5.03 3.5 3.5 5.03 3.5 6.91V9.22C3.5 9.64 3.16 9.97 2.75 9.97Z" fill="{color}"/>
<path d="M21.2493 9.97C20.8393 9.97 20.4993 9.63 20.4993 9.22V6.91C20.4993 5.03 18.9693 3.5 17.0893 3.5H14.7793C14.3693 3.5 14.0293 3.16 14.0293 2.75C14.0293 2.34 14.3593 2 14.7793 2H17.0893C19.7993 2 21.9993 4.2 21.9993 6.91V9.22C21.9993 9.64 21.6593 9.97 21.2493 9.97Z" fill="{color}"/>
<path d="M17.0892 22.0002H15.6992C15.2892 22.0002 14.9492 21.6602 14.9492 21.2502C14.9492 20.8402 15.2892 20.5002 15.6992 20.5002H17.0892C18.9692 20.5002 20.4992 18.9702 20.4992 17.0902V15.7002C20.4992 15.2902 20.8392 14.9502 21.2492 14.9502C21.6592 14.9502 21.9992 15.2902 21.9992 15.7002V17.0902C21.9992 19.8002 19.7992 22.0002 17.0892 22.0002Z" fill="{color}"/>
<path d="M9.22 21.9998H6.91C4.2 21.9998 2 19.7998 2 17.0898V14.7798C2 14.3698 2.34 14.0298 2.75 14.0298C3.16 14.0298 3.5 14.3698 3.5 14.7798V17.0898C3.5 18.9698 5.03 20.4998 6.91 20.4998H9.22C9.63 20.4998 9.97 20.8398 9.97 21.2498C9.97 21.6598 9.64 21.9998 9.22 21.9998Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2 9.75C1.59 9.75 1.25 9.41 1.25 9V6.5C1.25 3.61 3.61 1.25 6.5 1.25H9C9.41 1.25 9.75 1.59 9.75 2C9.75 2.41 9.41 2.75 9 2.75H6.5C4.43 2.75 2.75 4.43 2.75 6.5V9C2.75 9.41 2.41 9.75 2 9.75Z" fill="{color}"/>
<path d="M22 9.75C21.59 9.75 21.25 9.41 21.25 9V6.5C21.25 4.43 19.57 2.75 17.5 2.75H15C14.59 2.75 14.25 2.41 14.25 2C14.25 1.59 14.59 1.25 15 1.25H17.5C20.39 1.25 22.75 3.61 22.75 6.5V9C22.75 9.41 22.41 9.75 22 9.75Z" fill="{color}"/>
<path d="M17.5 22.75H16C15.59 22.75 15.25 22.41 15.25 22C15.25 21.59 15.59 21.25 16 21.25H17.5C19.57 21.25 21.25 19.57 21.25 17.5V16C21.25 15.59 21.59 15.25 22 15.25C22.41 15.25 22.75 15.59 22.75 16V17.5C22.75 20.39 20.39 22.75 17.5 22.75Z" fill="{color}"/>
<path d="M9 22.75H6.5C3.61 22.75 1.25 20.39 1.25 17.5V15C1.25 14.59 1.59 14.25 2 14.25C2.41 14.25 2.75 14.59 2.75 15V17.5C2.75 19.57 4.43 21.25 6.5 21.25H9C9.41 21.25 9.75 21.59 9.75 22C9.75 22.41 9.41 22.75 9 22.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2 9V6.5C2 4.01 4.01 2 6.5 2H9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M15 2H17.5C19.99 2 22 4.01 22 6.5V9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M22 16V17.5C22 19.99 19.99 22 17.5 22H16" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M9 22H6.5C4.01 22 2 19.99 2 17.5V15" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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