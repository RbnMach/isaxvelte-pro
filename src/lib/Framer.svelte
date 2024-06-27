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
<path d="M5 2L19 16H5V9H19V2H5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 16V22L5 16H12Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M4.5 10.4881V16.4281C4.5 16.7381 4.64 17.0381 4.87 17.2381L10.23 21.8281C10.93 22.4281 12 21.9281 12 21.0181V16.9181H16.91C17.86 16.9181 18.34 15.7681 17.67 15.0881L12 9.41812H5.57001C4.98001 9.40812 4.5 9.8881 4.5 10.4881Z" fill="{color}"/>
<path d="M18.4298 1.91016H7.0898C6.1398 1.91016 5.65979 3.06014 6.32979 3.74014L11.9998 9.41016H18.4298C19.0198 9.41016 19.4998 8.93015 19.4998 8.34015V2.98016C19.4998 2.39016 19.0198 1.91016 18.4298 1.91016Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5 10.52V9H19V2H5L19 16H5V15.22" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 16V22L5 16H12Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" d="M6 13.987v7.92c0 0.413 0.187 0.813 0.493 1.080l7.147 6.12c0.933 0.8 2.36 0.133 2.36-1.080v-5.467h6.547c1.267 0 1.907-1.533 1.013-2.44l-7.56-7.56h-8.573c-0.787-0.013-1.427 0.627-1.427 1.427z"></path>
<path fill="{color}" opacity="0.4" d="M24.573 2.547h-15.12c-1.267 0-1.907 1.533-1.013 2.44l7.56 7.56h8.573c0.787 0 1.427-0.64 1.427-1.427v-7.147c0-0.787-0.64-1.427-1.427-1.427z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M19 16.75H5C4.59 16.75 4.25 16.41 4.25 16V9C4.25 8.59 4.59 8.25 5 8.25H10.19L4.47 2.53C4.26 2.32 4.19 1.98999 4.31 1.70999C4.43 1.42999 4.7 1.25 5 1.25H19C19.41 1.25 19.75 1.59 19.75 2V9C19.75 9.41 19.41 9.75 19 9.75H13.81L19.53 15.47C19.74 15.68 19.81 16.01 19.69 16.29C19.57 16.57 19.3 16.75 19 16.75ZM5.75 15.25H17.19L11.69 9.75H5.75V15.25ZM12.31 8.25H18.25V2.75H6.81L12.31 8.25Z" fill="{color}"/>
<path d="M12.0001 22.75C11.8201 22.75 11.6502 22.69 11.5102 22.57L4.51015 16.57C4.27015 16.37 4.19015 16.03 4.29015 15.74C4.40015 15.45 4.68013 15.25 4.99013 15.25H11.9901C12.4001 15.25 12.7401 15.59 12.7401 16V22C12.7401 22.29 12.5701 22.56 12.3001 22.68C12.2101 22.73 12.1101 22.75 12.0001 22.75ZM7.03014 16.75L11.2501 20.37V16.75H7.03014Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5 2L19 16H5V9H19V2H5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M12 16V22L5 16H12Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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