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
<path d="M10.5 11.5V14.3L8 15.8L5.5 14.3V11.5L8 10L9.2 10.7L10.5 11.5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
<path d="M18.5 11.5V14.3L16 15.8L13.5 14.3V11.5L14.8 10.7L16 10L18.5 11.5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
<path d="M14.8002 9.30005V10.7L13.5002 11.5V13.2L12.0002 14.1L10.5002 13.2V11.5L9.2002 10.7V9.30005L12.0002 7.80005L14.8002 9.30005Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM18.5 14.02C18.5 14.2 18.4 14.36 18.25 14.45L16.25 15.6C16.1 15.69 15.91 15.69 15.75 15.6L13.75 14.45C13.59 14.36 13.5 14.2 13.5 14.02V13.19L12.25 13.91C12.1 14 11.91 14 11.75 13.91L10.5 13.19V14.02C10.5 14.2 10.4 14.36 10.25 14.45L8.25 15.6C8.1 15.69 7.91 15.69 7.75 15.6L5.75 14.45C5.59 14.36 5.5 14.2 5.5 14.02V11.74C5.5 11.56 5.6 11.4 5.75 11.31L7.75 10.16C7.9 10.07 8.1 10.07 8.25 10.16L9.25 10.74V9.61C9.25 9.43 9.35 9.26999 9.5 9.17999L11.75 7.89C11.9 7.8 12.09 7.8 12.25 7.89L14.5 9.17999C14.66 9.26999 14.75 9.43 14.75 9.61V10.74L15.75 10.16C15.9 10.07 16.09 10.07 16.25 10.16L18.25 11.31C18.41 11.4 18.5 11.56 18.5 11.74V14.02Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M10.5 11.46V14.31L8 15.75L5.5 14.31V11.46L8 10.02L9.25 10.74L10.5 11.46Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
<path d="M18.5 11.46V14.31L16 15.75L13.5 14.31V11.46L14.75 10.74L16 10.02L18.5 11.46Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
<path d="M14.75 9.33V10.74L13.5 11.46V13.19L12 14.05L10.5 13.19V11.46L9.25 10.74V9.33L12 7.75L14.75 9.33Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.19997 2.30001 7.96997 2.85001" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M14 15.28v3.427c0 0.24-0.133 0.453-0.333 0.573l-2.667 1.533c-0.2 0.12-0.453 0.12-0.667 0l-2.667-1.533c-0.213-0.12-0.333-0.333-0.333-0.573v-3.040c0-0.24 0.133-0.453 0.333-0.573l2.667-1.533c0.2-0.12 0.467-0.12 0.667 0l1.333 0.773 1.667 0.947z"></path>
<path fill="{color}" d="M24.667 15.667v3.040c0 0.24-0.133 0.453-0.333 0.573l-2.667 1.533c-0.2 0.12-0.453 0.12-0.667 0l-2.667-1.533c-0.213-0.12-0.333-0.333-0.333-0.573v-3.427l1.667-0.947 1.333-0.773c0.2-0.12 0.453-0.12 0.667 0l2.667 1.533c0.2 0.107 0.333 0.333 0.333 0.573z"></path>
<path fill="{color}" d="M19.667 12.827v1.507l-1.667 0.947v2.307l-1.667 0.96c-0.2 0.12-0.453 0.12-0.667 0l-1.667-0.96v-2.307l-1.667-0.947v-1.507c0-0.24 0.133-0.453 0.333-0.573l3-1.72c0.2-0.12 0.453-0.12 0.667 0l3 1.72c0.2 0.107 0.333 0.333 0.333 0.573z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M8 16.5C7.87 16.5 7.74 16.47 7.63 16.4L5.13 14.96C4.9 14.83 4.75 14.58 4.75 14.31V11.46C4.75 11.19 4.89 10.94 5.13 10.81L7.63 9.36996C7.86 9.23996 8.15 9.23996 8.38 9.36996L10.88 10.81C11.11 10.94 11.26 11.19 11.26 11.46V14.31C11.26 14.58 11.12 14.83 10.88 14.96L8.38 16.4C8.26 16.47 8.13 16.5 8 16.5ZM6.25 13.88L8 14.89L9.75 13.88V11.89L8 10.88L6.25 11.89V13.88Z" fill="{color}"/>
<path d="M16 16.5C15.87 16.5 15.74 16.47 15.63 16.4L13.13 14.96C12.9 14.83 12.75 14.58 12.75 14.31V11.46C12.75 11.19 12.89 10.94 13.13 10.81L15.63 9.36996C15.86 9.23996 16.15 9.23996 16.38 9.36996L18.88 10.81C19.11 10.94 19.26 11.19 19.26 11.46V14.31C19.26 14.58 19.12 14.83 18.88 14.96L16.38 16.4C16.26 16.47 16.13 16.5 16 16.5ZM14.25 13.88L16 14.89L17.75 13.88V11.89L16 10.88L14.25 11.89V13.88Z" fill="{color}"/>
<path d="M12 14.8002C11.87 14.8002 11.74 14.7702 11.63 14.7002L10.13 13.8402C9.9 13.7102 9.75 13.4602 9.75 13.1902V11.8902L8.88 11.3902C8.65 11.2602 8.5 11.0102 8.5 10.7402V9.32019C8.5 9.05019 8.64 8.80018 8.88 8.67018L11.63 7.09018C11.86 6.96018 12.15 6.96018 12.38 7.09018L15.13 8.67018C15.36 8.80018 15.51 9.05019 15.51 9.32019V10.7402C15.51 11.0102 15.37 11.2602 15.13 11.3902L14.26 11.8902V13.1902C14.26 13.4602 14.12 13.7102 13.88 13.8402L12.38 14.7002C12.26 14.7702 12.13 14.8002 12 14.8002ZM11.25 12.7602L12 13.1902L12.75 12.7602V11.4602C12.75 11.1902 12.89 10.9402 13.13 10.8102L14 10.3102V9.76017L12 8.61018L10 9.76017V10.3102L10.87 10.8102C11.1 10.9402 11.25 11.1902 11.25 11.4602V12.7602Z" fill="{color}"/>
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<g opacity="0.4">
<path d="M10.5 11.46V14.31L8 15.75L5.5 14.31V11.46L8 10.02L9.25 10.74L10.5 11.46Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
<path d="M18.5 11.46V14.31L16 15.75L13.5 14.31V11.46L14.75 10.74L16 10.02L18.5 11.46Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
<path d="M14.75 9.33V10.74L13.5 11.46V13.19L12 14.05L10.5 13.19V11.46L9.25 10.74V9.33L12 7.75L14.75 9.33Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
</g>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
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