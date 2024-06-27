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
<path d="M10.8999 2L0.899902 12L10.8999 22V18L4.8999 12L10.8999 6V2Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12.8999 2L22.8999 12L12.8999 22V18L18.8999 12L12.8999 6V2Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10.8999 9L7.8999 12L10.8999 15V9Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M10.0494 2.84808L1.25938 11.6381C1.05938 11.8381 1.05938 12.1481 1.25938 12.3481L10.0494 21.1381C10.3694 21.4481 10.8994 21.2281 10.8994 20.7881V18.1981C10.8994 18.0681 10.8494 17.9381 10.7494 17.8481L5.24937 12.3481C5.04937 12.1481 5.04937 11.8381 5.24937 11.6381L10.7494 6.13809C10.8394 6.04809 10.8994 5.91808 10.8994 5.78808V3.19808C10.8994 2.75808 10.3594 2.53808 10.0494 2.84808Z" fill="{color}"/>
<path d="M13.7504 2.84808L22.5403 11.6381C22.7403 11.8381 22.7403 12.1481 22.5403 12.3481L13.7504 21.1381C13.4404 21.4481 12.9004 21.2281 12.9004 20.7881V18.1981C12.9004 18.0681 12.9504 17.9381 13.0504 17.8481L18.5504 12.3481C18.7504 12.1481 18.7504 11.8381 18.5504 11.6381L13.0504 6.13809C12.9604 6.04809 12.9004 5.91808 12.9004 5.78808V3.19808C12.9004 2.75808 13.4404 2.53808 13.7504 2.84808Z" fill="{color}"/>
<path d="M10.0494 9.84808L8.25938 11.6381C8.05938 11.8381 8.05938 12.1481 8.25938 12.3481L10.0494 14.1381C10.3694 14.4481 10.8994 14.2281 10.8994 13.7881V10.1981C10.8994 9.75808 10.3594 9.53808 10.0494 9.84808Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M10.9004 2L0.900391 12L10.9004 22V18L4.90039 12L10.9004 6V2Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M18.9604 8.06L22.9004 12L12.9004 22V18L18.9004 12L12.9004 6V2L15.9404 5.04001" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10.9004 9L7.90039 12L10.9004 15V9Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M13.399 3.8l-11.72 11.72c-0.267 0.267-0.267 0.68 0 0.947l11.72 11.72c0.427 0.413 1.133 0.12 1.133-0.467v-3.453c0-0.173-0.067-0.347-0.2-0.467l-7.333-7.333c-0.267-0.267-0.267-0.68 0-0.947l7.333-7.333c0.12-0.12 0.2-0.293 0.2-0.467v-3.453c0-0.587-0.72-0.88-1.133-0.467z"></path>
<path fill="{color}" d="M18.334 3.8l11.72 11.72c0.267 0.267 0.267 0.68 0 0.947l-11.72 11.72c-0.413 0.413-1.133 0.12-1.133-0.467v-3.453c0-0.173 0.067-0.347 0.2-0.467l7.333-7.333c0.267-0.267 0.267-0.68 0-0.947l-7.333-7.333c-0.12-0.12-0.2-0.293-0.2-0.467v-3.453c0-0.587 0.72-0.88 1.133-0.467z"></path>
<path fill="{color}" d="M13.399 13.133l-2.387 2.387c-0.267 0.267-0.267 0.68 0 0.947l2.387 2.387c0.427 0.413 1.133 0.12 1.133-0.467v-4.787c0-0.587-0.72-0.88-1.133-0.467z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M10.8999 22.75C10.6999 22.75 10.5098 22.67 10.3698 22.53L0.369844 12.53C0.0798438 12.24 0.0798438 11.76 0.369844 11.47L10.3698 1.46999C10.5798 1.25999 10.9099 1.18999 11.1899 1.30999C11.4699 1.42999 11.6499 1.69999 11.6499 1.99999V5.99999C11.6499 6.19999 11.5698 6.38999 11.4298 6.52999L5.95987 12L11.4298 17.47C11.5698 17.61 11.6499 17.8 11.6499 18V22C11.6499 22.3 11.4699 22.58 11.1899 22.69C11.0899 22.73 10.9999 22.75 10.8999 22.75ZM1.95987 12L10.1499 20.19V18.31L4.36984 12.53C4.07984 12.24 4.07984 11.76 4.36984 11.47L10.1499 5.68999V3.80999L1.95987 12Z" fill="{color}"/>
<path d="M12.9004 22.75C12.8004 22.75 12.7104 22.73 12.6104 22.69C12.3304 22.57 12.1504 22.3 12.1504 22V18C12.1504 17.8 12.2304 17.61 12.3704 17.47L17.8404 12L12.3704 6.52999C12.2304 6.38999 12.1504 6.19999 12.1504 5.99999V1.99999C12.1504 1.69999 12.3304 1.41999 12.6104 1.30999C12.8904 1.18999 13.2104 1.25999 13.4304 1.46999L23.4304 11.47C23.7204 11.76 23.7204 12.24 23.4304 12.53L13.4304 22.53C13.2904 22.67 13.1004 22.75 12.9004 22.75ZM13.6504 18.31V20.19L21.8404 12L13.6504 3.80999V5.68999L19.4304 11.47C19.7204 11.76 19.7204 12.24 19.4304 12.53L13.6504 18.31Z" fill="{color}"/>
<path d="M10.8999 15.75C10.6999 15.75 10.5098 15.67 10.3698 15.53L7.36984 12.53C7.07984 12.24 7.07984 11.76 7.36984 11.47L10.3698 8.46999C10.5798 8.25999 10.9099 8.18999 11.1899 8.30999C11.4699 8.42999 11.6499 8.69999 11.6499 8.99999V15C11.6499 15.3 11.4699 15.58 11.1899 15.69C11.0899 15.73 10.9999 15.75 10.8999 15.75ZM8.95987 12L10.1499 13.19V10.81L8.95987 12Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M10.9004 2L0.900391 12L10.9004 22V18L4.90039 12L10.9004 6V2Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12.9004 2L22.9004 12L12.9004 22V18L18.9004 12L12.9004 6V2Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M10.9004 9L7.90039 12L10.9004 15V9Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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