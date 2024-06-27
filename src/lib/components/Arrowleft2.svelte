<script lang="ts">
	export let classes = '';
	export let color = 'currentColor';
	export let type: 'linear' | 'bold' | 'broken' | 'bulk' | 'outline' | 'twotone' = 'linear';
	export let size = '1em';
	export let axis_y = '-0.13em';
	export let axis_x = '0';
</script>

<span style="width: {size}; height: {size}; bottom: {axis_y}; left: {axis_x};" class={classes}>
	{#if type == 'linear'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15 19.9201L8.47997 13.4001C7.70997 12.6301 7.70997 11.3701 8.47997 10.6001L15 4.08008" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M13.9783 5.31877L10.7683 8.52877L8.79828 10.4888C7.96828 11.3188 7.96828 12.6688 8.79828 13.4988L13.9783 18.6788C14.6583 19.3588 15.8183 18.8688 15.8183 17.9188V12.3088V6.07877C15.8183 5.11877 14.6583 4.63877 13.9783 5.31877Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11.1897 7.93994L8.56969 10.5599C7.79969 11.3299 7.79969 12.5899 8.56969 13.3599L15.0897 19.8799" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.0908 4.04004L14.0508 5.08004" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M10.7702 8.52002L15.8202 12.31V17.92C15.8202 18.88 14.6602 19.36 13.9802 18.68L8.80023 13.51C7.97023 12.68 7.97023 11.33 8.80023 10.5L10.7702 8.52002Z" fill="{color}"/>
<path d="M15.8195 6.07993V12.3099L10.7695 8.51993L13.9795 5.30993C14.6595 4.63993 15.8195 5.11993 15.8195 6.07993Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M14.9993 20.67C14.8093 20.67 14.6193 20.6 14.4693 20.45L7.9493 13.93C6.8893 12.87 6.8893 11.13 7.9493 10.07L14.4693 3.55002C14.7593 3.26002 15.2393 3.26002 15.5293 3.55002C15.8193 3.84002 15.8193 4.32002 15.5293 4.61002L9.0093 11.13C8.5293 11.61 8.5293 12.39 9.0093 12.87L15.5293 19.39C15.8193 19.68 15.8193 20.16 15.5293 20.45C15.3793 20.59 15.1893 20.67 14.9993 20.67Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M14.9998 19.9201L8.47984 13.4001C7.70984 12.6301 7.70984 11.3701 8.47984 10.6001L14.9998 4.08008" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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
</style>