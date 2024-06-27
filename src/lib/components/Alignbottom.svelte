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
<path d="M19.26 18.9V7.1C19.26 5.6 18.62 5 17.03 5H15.99C14.4 5 13.76 5.6 13.76 7.1V18.9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5.25999 18.9V12.1C5.25999 10.6 5.89999 10 7.48999 10H8.52999C10.12 10 10.76 10.6 10.76 12.1V18.9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 19H22" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <path d="M13.75,6.74v11.88s5.5,0,5.5,0V6.74c0-1.52-.64-2.12-2.23-2.12h-1.04c-1.58,0-2.22.6-2.23,2.12Z" fill="{color}" stroke-width="0"/>
  <path d="M5.25,11.74v6.88s5.5,0,5.5,0v-6.88c0-1.51-.64-2.12-2.23-2.12h-1.04c-1.58,0-2.23.61-2.23,2.12Z" fill="{color}" stroke-width="0"/>
  <path d="M22,18.62c0,.42-.34.76-.75.76H2.75c-.41,0-.75-.34-.75-.75s.34-.75.75-.75h18.5c.41,0,.75.32.75.74Z" fill="{color}" stroke-width="0"/>
</svg>
	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M19.2598 18.9V7.1C19.2598 5.6 18.6198 5 17.0298 5H15.9898C14.3998 5 13.7598 5.6 13.7598 7.1V18.9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10.7598 12.1001V18.9001" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5.25977 18.9V12.1C5.25977 10.6 5.89977 10 7.48977 10" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 19H22" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <path d="M13.75,6.74v11.88s5.5,0,5.5,0V6.74c0-1.52-.64-2.12-2.23-2.12h-1.04c-1.58,0-2.22.6-2.23,2.12Z" fill="{color}" stroke-width="0"/>
  <path d="M5.25,11.74v6.88s5.5,0,5.5,0v-6.88c0-1.51-.64-2.12-2.23-2.12h-1.04c-1.58,0-2.23.61-2.23,2.12Z" fill="{color}" isolation="isolate" opacity=".4" stroke-width="0"/>
  <path d="M22,18.62c0,.42-.34.76-.75.76H2.75c-.41,0-.75-.34-.75-.75s.34-.75.75-.75h18.5c.41,0,.75.32.75.74Z" fill="{color}" stroke-width="0"/>
</svg>
	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M19.2598 19.65C18.8498 19.65 18.5098 19.31 18.5098 18.9V7.1C18.5098 6.09 18.2998 5.75 17.0298 5.75H15.9898C14.7198 5.75 14.5098 6.09 14.5098 7.1V18.9C14.5098 19.31 14.1698 19.65 13.7598 19.65C13.3498 19.65 13.0098 19.31 13.0098 18.9V7.1C13.0098 5.18 13.9898 4.25 15.9898 4.25H17.0298C19.0398 4.25 20.0098 5.18 20.0098 7.1V18.9C20.0098 19.31 19.6698 19.65 19.2598 19.65Z" fill="{color}"/>
<path d="M10.7598 19.65C10.3498 19.65 10.0098 19.31 10.0098 18.9V12.1C10.0098 11.09 9.79977 10.75 8.52977 10.75H7.48977C6.21977 10.75 6.00977 11.09 6.00977 12.1V18.9C6.00977 19.31 5.66977 19.65 5.25977 19.65C4.84977 19.65 4.50977 19.31 4.50977 18.9V12.1C4.50977 10.18 5.48977 9.25 7.48977 9.25H8.52977C10.5398 9.25 11.5098 10.18 11.5098 12.1V18.9C11.5098 19.31 11.1698 19.65 10.7598 19.65Z" fill="{color}"/>
<path d="M22 19.75H2C1.59 19.75 1.25 19.41 1.25 19C1.25 18.59 1.58 18.25 2 18.25H22C22.41 18.25 22.75 18.59 22.75 19C22.75 19.41 22.42 19.75 22 19.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M19.2598 18.9V7.1C19.2598 5.6 18.6198 5 17.0298 5H15.9898C14.3998 5 13.7598 5.6 13.7598 7.1V18.9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M5.25977 18.9V12.1C5.25977 10.6 5.89977 10 7.48977 10H8.52977C10.1198 10 10.7598 10.6 10.7598 12.1V18.9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 19H22" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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