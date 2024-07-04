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
  <path d="M13.8,21.8c4.4-.8,7.8-4.5,8.1-9.1.5-5.5-3.6-10.3-9.2-10.7C6.1,1.5,2.3,6.8,2.3,6.8M2.3,6.8l.3-4.5M2.3,6.8l2,.1,2.4.2" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
  <path d="M2,11.3c-.81,5.14,4.95,11.94,11.8,10.5" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
  <path d="M15.4,15.8l-3.2-1.8c-.5-.3-1-1.1-1-1.7v-4.1" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
</svg>
	{/if}
	{#if variant == 'bold'}
		<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <path d="M13.8,21.8c4.4-.8,7.8-4.5,8.1-9.1.5-5.5-3.6-10.3-9.2-10.7C6.1,1.5,2.3,6.8,2.3,6.8M2.3,6.8l.3-4.5M2.3,6.8l2,.1,2.4.2" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
  <path d="M2,11.3c-.81,5.14,4.95,11.94,11.8,10.5" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
  <path d="M15.4,15.8l-3.2-1.8c-.5-.3-1-1.1-1-1.7v-4.1" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
</svg>
	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M13.8,21.8c4.4-.8,7.8-4.5,8.1-9.1.5-5.5-3.6-10.3-9.2-10.7C6.1,1.5,2.3,6.8,2.3,6.8M2.3,6.8l.3-4.5M2.3,6.8l2,.1,2.4.2"  stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
  <path d="M2,11.3c-.4,5.5,3.8,10.3,9.3,10.7"  stroke="{color}" stroke-dasharray="0 0 4 5" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
  <path d="M15.4,15.8l-3.2-1.8c-.5-.3-1-1.1-1-1.7v-4.1"  stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
</svg>
	{/if}										
	{#if variant == 'bulk'}
		<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <path d="M13.8,21.8c4.4-.8,7.8-4.5,8.1-9.1.5-5.5-3.6-10.3-9.2-10.7C6.1,1.5,2.3,6.8,2.3,6.8M2.3,6.8l.3-4.5M2.3,6.8l2,.1,2.4.2" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
  <path d="M2,11.3c-.81,5.14,4.95,11.94,11.8,10.5" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
  <path d="M15.4,15.8l-3.2-1.8c-.5-.3-1-1.1-1-1.7v-4.1" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
  <path opacity="0.4" d="M11.9707 22C17.4936 22 21.9707 17.5228 21.9707 12C21.9707 6.47715 17.4936 2 11.9707 2C6.44786 2 1.9707 6.47715 1.9707 12C1.9707 17.5228 6.44786 22 11.9707 22Z" fill="{color}"/>
</svg>
	{/if}										
	{#if variant == 'outline'}
		<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <path d="M13.8,21.8c4.4-.8,7.8-4.5,8.1-9.1.5-5.5-3.6-10.3-9.2-10.7C6.1,1.5,2.3,6.8,2.3,6.8M2.3,6.8l.3-4.5M2.3,6.8l2,.1,2.4.2" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
  <path d="M2,11.3c-.81,5.14,4.95,11.94,11.8,10.5" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
  <path d="M15.4,15.8l-3.2-1.8c-.5-.3-1-1.1-1-1.7v-4.1" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
</svg>
	{/if}										
	{#if variant == 'twotone'}
		<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <path d="M13.8,21.8c4.4-.8,7.8-4.5,8.1-9.1.5-5.5-3.6-10.3-9.2-10.7C6.1,1.5,2.3,6.8,2.3,6.8M2.3,6.8l.3-4.5M2.3,6.8l2,.1,2.4.2" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
  <path opacity="0.4" d="M2,11.3c-.81,5.14,4.95,11.94,11.8,10.5" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
  <path d="M15.4,15.8l-3.2-1.8c-.5-.3-1-1.1-1-1.7v-4.1" fill="none" stroke="{color}" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"/>
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