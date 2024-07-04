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
		<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <path d="M6.32,9.5l-2.56,2.56,2.56,2.56" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
  <path d="M3.83,12.06h10.17" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
  <path d="M12,4c4.42,0,8,3,8,8s-3.58,8-8,8" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
</svg>
	{/if}
	{#if variant == 'bold'}
		<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <path d="M15.37,12.81h-5.47s0,8.33,0,8.33c0,.48.39.86.86.86,5.89,0,10-4.11,10-10,0-5.89-4.11-10-10-10-.48,0-.86.38-.87.86v8.46s5.48,0,5.48,0c.41,0,.75.34.75.75,0,.41-.33.75-.75.74Z" fill="{color}" stroke-width="0"/>
  <path d="M3.46,12.58l2.84,2.85c.15.15.34.22.53.22s.38-.07.53-.22c.29-.29.29-.77,0-1.06l-1.56-1.56h4.09s0-1.5,0-1.5h-4.1s1.56-1.56,1.56-1.56c.29-.29.29-.77,0-1.06-.29-.29-.77-.29-1.06,0l-2.84,2.85c-.29.29-.29.76,0,1.04Z" fill="{color}" stroke-width="0"/>
</svg>
	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M6.56 14.5599L4 11.9999L6.56 9.43994" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9.24031 12H4.07031" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M14.2393 12H12.2793" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M18.01 6.47998C19.25 7.83998 20 9.70998 20 12C20 17 16.42 20 12 20" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 4C13.05 4 14.05 4.17 14.97 4.49" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <path d="M20.76,12.01c0,5.89-4.11,10-10,10-.48,0-.86-.39-.86-.86V2.86c0-.48.39-.86.86-.86,5.88,0,10,4.12,10,10.01Z" fill="{color}" isolation="isolate" opacity=".4" stroke-width="0"/>
  <path d="M3.46,12.58l2.84,2.85c.15.15.34.22.53.22s.38-.07.53-.22c.29-.29.29-.77,0-1.06l-1.56-1.56h9.57c.41,0,.75-.34.75-.75s-.34-.75-.75-.75H5.8s1.56-1.56,1.56-1.56c.29-.29.29-.77,0-1.06-.29-.29-.77-.29-1.06,0l-2.84,2.85c-.29.29-.29.76,0,1.04Z" fill="{color}" stroke-width="0"/>
</svg>
	{/if}										
	{#if variant == 'outline'}
		<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <path d="M5.79,15.15l-2.56-2.56c-.29-.29-.29-.77,0-1.06l2.56-2.56c.29-.29.77-.29,1.06,0,.29.29.29.77,0,1.06l-2.03,2.03,2.03,2.03c.29.29.29.77,0,1.06-.15.15-.34.22-.53.22s-.38-.07-.53-.22Z" fill="{color}" stroke-width="0"/>
  <path d="M3.08,12.06c0-.41.34-.75.75-.75h10.17c.41,0,.75.34.75.75s-.34.75-.75.75H3.83c-.41,0-.75-.34-.75-.75Z" fill="{color}" stroke-width="0"/>
  <path d="M11.25,20c0-.41.34-.75.75-.75,4.27,0,7.25-2.98,7.25-7.25s-2.98-7.25-7.25-7.25c-.41,0-.75-.34-.75-.75s.34-.75.75-.75c5.15,0,8.75,3.6,8.75,8.75,0,5.15-3.6,8.75-8.75,8.75-.41,0-.75-.34-.75-.75Z" fill="{color}" stroke-width="0"/>
</svg>
	{/if}										
	{#if variant == 'twotone'}
		<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <g opacity=".4">
    <path d="M6.32,9.5l-2.56,2.56,2.56,2.56" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
    <path d="M3.83,12.06h10.17" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
  </g>
  <path d="M12,4c4.42,0,8,3,8,8s-3.58,8-8,8" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
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