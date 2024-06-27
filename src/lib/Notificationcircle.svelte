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
<path d="M19 8C20.6569 8 22 6.65685 22 5C22 3.34315 20.6569 2 19 2C17.3431 2 16 3.34315 16 5C16 6.65685 17.3431 8 19 8Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M14.02 2.2C13.36 2.07 12.69 2 12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 11.32 21.93 10.65 21.8 10.01" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M19 8C20.6569 8 22 6.65685 22 5C22 3.34315 20.6569 2 19 2C17.3431 2 16 3.34315 16 5C16 6.65685 17.3431 8 19 8Z" fill="{color}"/>
<path d="M17.7892 9.33927C16.2792 8.93927 15.0592 7.71927 14.6592 6.20927C14.3992 5.24927 14.4592 4.32927 14.7492 3.50927C14.9492 2.94927 14.6092 2.32927 14.0292 2.20927C12.5592 1.89927 10.9692 1.90927 9.30923 2.35927C5.52923 3.41927 2.63923 6.68927 2.09923 10.5793C1.17923 17.1993 6.78923 22.8093 13.4092 21.8993C17.3092 21.3593 20.5692 18.4693 21.6192 14.6793C22.0792 13.0293 22.0892 11.4393 21.7792 9.95927C21.6592 9.37927 21.0392 9.04927 20.4792 9.23927C19.6692 9.52927 18.7492 9.58927 17.7892 9.33927Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M3.01953 16.3998C4.63953 19.7198 8.04953 21.9998 11.9995 21.9998C17.5195 21.9998 21.9995 17.5198 21.9995 11.9998C21.9995 11.3198 21.9295 10.6498 21.7995 10.0098" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M14.02 2.2C13.36 2.07 12.69 2 12 2C6.48 2 2 6.48 2 12" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M19 2C17.34 2 16 3.34 16 5C16 6.66 17.34 8 19 8C20.66 8 22 6.66 22 5C22 4.64 21.94 4.3 21.82 3.99" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M19 8C20.6569 8 22 6.65685 22 5C22 3.34315 20.6569 2 19 2C17.3431 2 16 3.34315 16 5C16 6.65685 17.3431 8 19 8Z" fill="{color}"/>
<path opacity="0.4" d="M19 9.5C16.52 9.5 14.5 7.48 14.5 5C14.5 4.09 14.77 3.25 15.24 2.55C14.22 2.2 13.13 2 12 2C6.49 2 2 6.49 2 12C2 17.51 6.49 22 12 22C17.51 22 22 17.51 22 12C22 10.87 21.8 9.78 21.45 8.76C20.75 9.23 19.91 9.5 19 9.5Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M19 8.75C16.93 8.75 15.25 7.07 15.25 5C15.25 2.93 16.93 1.25 19 1.25C21.07 1.25 22.75 2.93 22.75 5C22.75 7.07 21.07 8.75 19 8.75ZM19 2.75C17.76 2.75 16.75 3.76 16.75 5C16.75 6.24 17.76 7.25 19 7.25C20.24 7.25 21.25 6.24 21.25 5C21.25 3.76 20.24 2.75 19 2.75Z" fill="{color}"/>
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C12.73 1.25 13.46 1.32 14.17 1.47C14.58 1.55 14.84 1.95 14.75 2.36C14.67 2.77 14.27 3.03 13.87 2.94C13.26 2.81 12.63 2.75 12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 11.38 21.19 10.76 21.07 10.16C20.99 9.75 21.25 9.36 21.66 9.28C22.07 9.19 22.46 9.46 22.54 9.87C22.68 10.57 22.75 11.29 22.75 12.01C22.75 17.93 17.93 22.75 12 22.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M19 8C20.6569 8 22 6.65685 22 5C22 3.34315 20.6569 2 19 2C17.3431 2 16 3.34315 16 5C16 6.65685 17.3431 8 19 8Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M14.02 2.2C13.36 2.07 12.69 2 12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 11.32 21.93 10.65 21.8 10.01" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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