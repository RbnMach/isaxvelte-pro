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
<path d="M3 4.5H21" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.53 9.5H21" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3 14.5H21" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.53 19.5H21" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M21 5.25H3C2.59 5.25 2.25 4.91 2.25 4.5C2.25 4.09 2.59 3.75 3 3.75H21C21.41 3.75 21.75 4.09 21.75 4.5C21.75 4.91 21.41 5.25 21 5.25Z" fill="{color}"/>
<path d="M21.0013 10.25H11.5312C11.1213 10.25 10.7812 9.91 10.7812 9.5C10.7812 9.09 11.1213 8.75 11.5312 8.75H21.0013C21.4113 8.75 21.7513 9.09 21.7513 9.5C21.7513 9.91 21.4113 10.25 21.0013 10.25Z" fill="{color}"/>
<path d="M21 15.25H3C2.59 15.25 2.25 14.91 2.25 14.5C2.25 14.09 2.59 13.75 3 13.75H21C21.41 13.75 21.75 14.09 21.75 14.5C21.75 14.91 21.41 15.25 21 15.25Z" fill="{color}"/>
<path d="M21.0013 20.25H11.5312C11.1213 20.25 10.7812 19.91 10.7812 19.5C10.7812 19.09 11.1213 18.75 11.5312 18.75H21.0013C21.4113 18.75 21.7513 19.09 21.7513 19.5C21.7513 19.91 21.4113 20.25 21.0013 20.25Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11.5293 9.5H20.9993" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3 14.5H21" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.5293 19.5H20.9993" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M13.95 4.5H3" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M20.9995 4.5H18.0195" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M21 5.25H3C2.59 5.25 2.25 4.91 2.25 4.5C2.25 4.09 2.59 3.75 3 3.75H21C21.41 3.75 21.75 4.09 21.75 4.5C21.75 4.91 21.41 5.25 21 5.25Z" fill="{color}"/>
<path opacity="0.4" d="M20.9993 10.25H11.5293C11.1193 10.25 10.7793 9.91 10.7793 9.5C10.7793 9.09 11.1193 8.75 11.5293 8.75H20.9993C21.4093 8.75 21.7493 9.09 21.7493 9.5C21.7493 9.91 21.4093 10.25 20.9993 10.25Z" fill="{color}"/>
<path d="M21 15.25H3C2.59 15.25 2.25 14.91 2.25 14.5C2.25 14.09 2.59 13.75 3 13.75H21C21.41 13.75 21.75 14.09 21.75 14.5C21.75 14.91 21.41 15.25 21 15.25Z" fill="{color}"/>
<path opacity="0.4" d="M20.9993 20.25H11.5293C11.1193 20.25 10.7793 19.91 10.7793 19.5C10.7793 19.09 11.1193 18.75 11.5293 18.75H20.9993C21.4093 18.75 21.7493 19.09 21.7493 19.5C21.7493 19.91 21.4093 20.25 20.9993 20.25Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M21 5.25H3C2.59 5.25 2.25 4.91 2.25 4.5C2.25 4.09 2.59 3.75 3 3.75H21C21.41 3.75 21.75 4.09 21.75 4.5C21.75 4.91 21.41 5.25 21 5.25Z" fill="{color}"/>
<path d="M20.9993 10.25H11.5293C11.1193 10.25 10.7793 9.91 10.7793 9.5C10.7793 9.09 11.1193 8.75 11.5293 8.75H20.9993C21.4093 8.75 21.7493 9.09 21.7493 9.5C21.7493 9.91 21.4093 10.25 20.9993 10.25Z" fill="{color}"/>
<path d="M21 15.25H3C2.59 15.25 2.25 14.91 2.25 14.5C2.25 14.09 2.59 13.75 3 13.75H21C21.41 13.75 21.75 14.09 21.75 14.5C21.75 14.91 21.41 15.25 21 15.25Z" fill="{color}"/>
<path d="M20.9993 20.25H11.5293C11.1193 20.25 10.7793 19.91 10.7793 19.5C10.7793 19.09 11.1193 18.75 11.5293 18.75H20.9993C21.4093 18.75 21.7493 19.09 21.7493 19.5C21.7493 19.91 21.4093 20.25 20.9993 20.25Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M3 4.5H21" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.5293 9.5H20.9993" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M3 14.5H21" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.5293 19.5H20.9993" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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