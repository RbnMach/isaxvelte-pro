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
<path d="M12 16C15.87 16 19 12.87 19 9C19 5.13 15.87 2 12 2C8.13 2 5 5.13 5 9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 16V22" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15 19H9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M19.75 9C19.75 4.73 16.27 1.25 12 1.25C7.73 1.25 4.25 4.73 4.25 9C4.25 9.41 4.59 9.75 5 9.75C5.41 9.75 5.75 9.41 5.75 9C5.75 5.55 8.55 2.75 12 2.75C15.45 2.75 18.25 5.55 18.25 9C18.25 12.45 15.45 15.25 12 15.25C11.59 15.25 11.25 15.59 11.25 16V22C11.25 22.41 11.59 22.75 12 22.75C12.41 22.75 12.75 22.41 12.75 22V16.71C16.67 16.33 19.75 13.02 19.75 9Z" fill="{color}"/>
<path d="M15 19.75H9C8.59 19.75 8.25 19.41 8.25 19C8.25 18.59 8.59 18.25 9 18.25H15C15.41 18.25 15.75 18.59 15.75 19C15.75 19.41 15.41 19.75 15 19.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 16C15.87 16 19 12.87 19 9C19 5.13 15.87 2 12 2C8.13 2 5 5.13 5 9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 16V22" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15 19H9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M19.75 9C19.75 4.73 16.27 1.25 12 1.25C7.73 1.25 4.25 4.73 4.25 9C4.25 9.41 4.59 9.75 5 9.75C5.41 9.75 5.75 9.41 5.75 9C5.75 5.55 8.55 2.75 12 2.75C15.45 2.75 18.25 5.55 18.25 9C18.25 12.45 15.45 15.25 12 15.25C11.59 15.25 11.25 15.59 11.25 16V22C11.25 22.41 11.59 22.75 12 22.75C12.41 22.75 12.75 22.41 12.75 22V16.71C16.67 16.33 19.75 13.02 19.75 9Z" fill="{color}"/>
<path opacity="0.4" d="M15 19.75H9C8.59 19.75 8.25 19.41 8.25 19C8.25 18.59 8.59 18.25 9 18.25H15C15.41 18.25 15.75 18.59 15.75 19C15.75 19.41 15.41 19.75 15 19.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 16.75C11.59 16.75 11.25 16.41 11.25 16C11.25 15.59 11.59 15.25 12 15.25C15.45 15.25 18.25 12.45 18.25 9C18.25 5.55 15.45 2.75 12 2.75C8.55 2.75 5.75 5.55 5.75 9C5.75 9.41 5.41 9.75 5 9.75C4.59 9.75 4.25 9.41 4.25 9C4.25 4.73 7.73 1.25 12 1.25C16.27 1.25 19.75 4.73 19.75 9C19.75 13.27 16.27 16.75 12 16.75Z" fill="{color}"/>
<path d="M12 22.75C11.59 22.75 11.25 22.41 11.25 22V16C11.25 15.59 11.59 15.25 12 15.25C12.41 15.25 12.75 15.59 12.75 16V22C12.75 22.41 12.41 22.75 12 22.75Z" fill="{color}"/>
<path d="M15 19.75H9C8.59 19.75 8.25 19.41 8.25 19C8.25 18.59 8.59 18.25 9 18.25H15C15.41 18.25 15.75 18.59 15.75 19C15.75 19.41 15.41 19.75 15 19.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 16C15.87 16 19 12.87 19 9C19 5.13 15.87 2 12 2C8.13 2 5 5.13 5 9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 16V22" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M15 19H9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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