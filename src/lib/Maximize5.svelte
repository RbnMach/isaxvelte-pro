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
<path d="M2 9.98V9C2 4 4 2 9 2H15C20 2 22 4 22 9V15C22 20 20 22 15 22H14" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M13 11L18.01 5.97998H14" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M18.01 5.97998V9.98998" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11 16.15V18.85C11 21.1 10.1 22 7.85 22H5.15C2.9 22 2 21.1 2 18.85V16.15C2 13.9 2.9 13 5.15 13H7.85C10.1 13 11 13.9 11 16.15Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11 16.15V18.85C11 21.1 10.1 22 7.85 22H5.15C2.9 22 2 21.1 2 18.85V16.15C2 13.9 2.9 13 5.15 13H7.85C10.1 13 11 13.9 11 16.15Z" fill="{color}"/>
<path d="M16.48 2H8.52C5.47 2 3 4.47 3 7.52V10.5C3 11.05 3.45 11.5 4 11.5H8.5C10.71 11.5 12.5 13.29 12.5 15.5V20C12.5 20.55 12.95 21 13.5 21H16.48C19.93 21 22 18.94 22 15.48V7.52C22 4.47 19.53 2 16.48 2ZM18.76 9.99C18.76 10.4 18.42 10.74 18.01 10.74C17.6 10.74 17.26 10.4 17.26 9.99V7.79L13.53 11.53C13.38 11.68 13.19 11.75 13 11.75C12.81 11.75 12.62 11.68 12.47 11.53C12.18 11.24 12.18 10.76 12.47 10.47L16.2 6.72H14C13.58 6.72 13.25 6.39 13.25 5.97C13.25 5.56 13.58 5.22 14 5.22H18.01C18.1 5.22 18.19 5.25 18.27 5.28C18.3 5.29 18.32 5.3 18.34 5.31C18.4 5.34 18.45 5.37 18.5 5.42C18.52 5.43 18.54 5.45 18.56 5.47C18.61 5.53 18.65 5.59 18.69 5.66C18.69 5.67 18.7 5.68 18.7 5.69C18.74 5.77 18.75 5.86 18.75 5.95C18.76 5.96 18.76 5.96 18.76 5.97V9.99Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2 9.98V9C2 4 4 2 9 2H15C20 2 22 4 22 9V15C22 20 20 22 15 22H14" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M13 11L18.01 5.97998H14" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M18.0098 5.97998V9.98998" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 18.85V16.15C2 13.9 2.9 13 5.15 13H7.85C10.1 13 11 13.9 11 16.15V18.85C11 21.1 10.1 22 7.85 22H5.15" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M16.48 2H8.52C5.07 2 3 4.06 3 7.52V15.47C3 18.94 5.07 21 8.52 21H16.47C19.93 21 21.99 18.94 21.99 15.48V7.52C22 4.06 19.93 2 16.48 2Z" fill="{color}"/>
<path d="M11 16.15V18.85C11 21.1 10.1 22 7.85 22H5.15C2.9 22 2 21.1 2 18.85V16.15C2 13.9 2.9 13 5.15 13H7.85C10.1 13 11 13.9 11 16.15Z" fill="{color}"/>
<path d="M18.7495 5.95C18.7495 5.86 18.7295 5.78 18.6995 5.69C18.6995 5.68 18.6895 5.67 18.6895 5.67C18.6595 5.6 18.6095 5.53 18.5595 5.48C18.5395 5.46 18.5195 5.44 18.4995 5.43C18.4495 5.39 18.3995 5.35 18.3495 5.33C18.3295 5.32 18.2995 5.31 18.2795 5.3C18.1995 5.27 18.1095 5.25 18.0195 5.25H13.9995C13.5895 5.25 13.2495 5.59 13.2495 6C13.2495 6.41 13.5795 6.72 13.9995 6.72H16.2095L12.4695 10.47C12.1795 10.76 12.1795 11.24 12.4695 11.53C12.6195 11.68 12.8095 11.75 12.9995 11.75C13.1895 11.75 13.3795 11.68 13.5295 11.53L17.2595 7.79V9.99C17.2595 10.4 17.5995 10.74 18.0095 10.74C18.4195 10.74 18.7595 10.4 18.7595 9.99V5.97C18.7595 5.96 18.7595 5.96 18.7495 5.95Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15 22.75H14C13.59 22.75 13.25 22.41 13.25 22C13.25 21.59 13.59 21.25 14 21.25H15C19.61 21.25 21.25 19.61 21.25 15V9C21.25 4.39 19.61 2.75 15 2.75H9C4.39 2.75 2.75 4.39 2.75 9V9.98C2.75 10.39 2.41 10.73 2 10.73C1.59 10.73 1.25 10.39 1.25 9.98V9C1.25 3.57 3.57 1.25 9 1.25H15C20.43 1.25 22.75 3.57 22.75 9V15C22.75 20.43 20.43 22.75 15 22.75Z" fill="{color}"/>
<path d="M12.9995 11.7502C12.8095 11.7502 12.6195 11.6802 12.4695 11.5302C12.1795 11.2402 12.1795 10.7602 12.4695 10.4702L16.2095 6.72021H13.9995C13.5895 6.72021 13.2495 6.38021 13.2495 5.97021C13.2495 5.56021 13.5795 5.22021 13.9995 5.22021H18.0095C18.3095 5.22021 18.5895 5.40021 18.6995 5.68021C18.8195 5.96021 18.7495 6.28022 18.5395 6.50022L13.5295 11.5302C13.3795 11.6802 13.1895 11.7502 12.9995 11.7502Z" fill="{color}"/>
<path d="M18.0098 10.7402C17.5998 10.7402 17.2598 10.4002 17.2598 9.99021V5.97021C17.2598 5.56021 17.5998 5.22021 18.0098 5.22021C18.4198 5.22021 18.7598 5.56021 18.7598 5.97021V9.98021C18.7598 10.4002 18.4198 10.7402 18.0098 10.7402Z" fill="{color}"/>
<path d="M7.85 22.75H5.15C2.49 22.75 1.25 21.51 1.25 18.85V16.15C1.25 13.49 2.49 12.25 5.15 12.25H7.85C10.51 12.25 11.75 13.49 11.75 16.15V18.85C11.75 21.51 10.51 22.75 7.85 22.75ZM5.15 13.75C3.31 13.75 2.75 14.31 2.75 16.15V18.85C2.75 20.69 3.31 21.25 5.15 21.25H7.85C9.69 21.25 10.25 20.69 10.25 18.85V16.15C10.25 14.31 9.69 13.75 7.85 13.75H5.15Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2 9.98V9C2 4 4 2 9 2H15C20 2 22 4 22 9V15C22 20 20 22 15 22H14" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<g opacity="0.4">
<path d="M13 11.0005L18.01 5.98047H14" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M18.0098 5.98047V9.99047" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</g>
<path opacity="0.4" d="M11 16.15V18.85C11 21.1 10.1 22 7.85 22H5.15C2.9 22 2 21.1 2 18.85V16.15C2 13.9 2.9 13 5.15 13H7.85C10.1 13 11 13.9 11 16.15Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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