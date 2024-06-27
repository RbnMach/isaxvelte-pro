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
<path d="M7.5 10.5H16.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9 6.5L11.8 10.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M14.8 6.5L12 10.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7.5 13.5H16.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9 17.5L11.8 13.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M14.8 17.5L12 13.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM16.5 14.25H13.45L15.44 17.07C15.68 17.41 15.6 17.88 15.26 18.11C15.13 18.2 14.98 18.25 14.83 18.25C14.59 18.25 14.36 18.14 14.22 17.93L11.92 14.67L9.62 17.93C9.47 18.14 9.24001 18.25 9.01001 18.25C8.86001 18.25 8.70999 18.21 8.57999 18.11C8.23999 17.87 8.15999 17.4 8.39999 17.07L10.39 14.25H7.51999C7.10999 14.25 6.76999 13.91 6.76999 13.5C6.76999 13.09 7.10999 12.75 7.51999 12.75H16.52C16.93 12.75 17.27 13.09 17.27 13.5C17.27 13.91 16.91 14.25 16.5 14.25ZM16.5 11.25H7.5C7.09 11.25 6.75 10.91 6.75 10.5C6.75 10.09 7.09 9.75 7.5 9.75H10.37L8.38 6.92999C8.14001 6.58999 8.22 6.12 8.56 5.89C8.9 5.65 9.37001 5.73001 9.60001 6.07001L11.9 9.33L14.2 6.07001C14.44 5.73001 14.91 5.65 15.24 5.89C15.58 6.13 15.66 6.59999 15.42 6.92999L13.43 9.75H16.48C16.89 9.75 17.23 10.09 17.23 10.5C17.23 10.91 16.91 11.25 16.5 11.25Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M7.5 10.5H16.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9 6.5L11.82 10.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M14.82 6.5L12 10.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7.5 13.5H16.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9 17.5L11.82 13.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M14.82 17.5L12 13.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.2 2.30001 7.97 2.85001" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M9.999 15h12c0.547 0 1-0.453 1-1s-0.453-1-1-1h-4.067l2.653-3.76c0.32-0.453 0.213-1.080-0.24-1.387-0.453-0.32-1.080-0.213-1.387 0.24l-3.067 4.347-3.067-4.347c-0.32-0.453-0.947-0.56-1.387-0.24-0.453 0.32-0.56 0.947-0.24 1.387l2.653 3.76h-3.827c-0.547 0-1 0.453-1 1s0.427 1 0.973 1z"></path>
<path fill="{color}" d="M22 17.001h-12c-0.547 0-1 0.453-1 1s0.453 1 1 1h3.827l-2.653 3.76c-0.32 0.453-0.213 1.080 0.24 1.387 0.173 0.12 0.373 0.187 0.573 0.187 0.32 0 0.627-0.147 0.813-0.427l3.067-4.347 3.067 4.347c0.2 0.28 0.507 0.427 0.813 0.427 0.2 0 0.4-0.053 0.573-0.187 0.453-0.32 0.56-0.947 0.24-1.387l-2.653-3.76h4.067c0.547 0 1-0.453 1-1s-0.427-1-0.973-1z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.5 11.25H7.5C7.09 11.25 6.75 10.91 6.75 10.5C6.75 10.09 7.09 9.75 7.5 9.75H16.5C16.91 9.75 17.25 10.09 17.25 10.5C17.25 10.91 16.91 11.25 16.5 11.25Z" fill="{color}"/>
<path d="M11.8203 11.2498C11.5803 11.2498 11.3503 11.1398 11.2103 10.9298L8.3903 6.9298C8.1503 6.5898 8.23029 6.11981 8.57029 5.88981C8.91029 5.64981 9.38027 5.72981 9.61027 6.06981L12.4303 10.0698C12.6703 10.4098 12.5903 10.8798 12.2503 11.1098C12.1203 11.2098 11.9703 11.2498 11.8203 11.2498Z" fill="{color}"/>
<path d="M12.0003 11.2498C11.8503 11.2498 11.7003 11.2098 11.5703 11.1098C11.2303 10.8698 11.1503 10.3998 11.3903 10.0698L14.2103 6.06981C14.4503 5.72981 14.9203 5.64981 15.2503 5.88981C15.5903 6.12981 15.6703 6.5998 15.4303 6.9298L12.6103 10.9298C12.4703 11.1398 12.2303 11.2498 12.0003 11.2498Z" fill="{color}"/>
<path d="M16.5 14.25H7.5C7.09 14.25 6.75 13.91 6.75 13.5C6.75 13.09 7.09 12.75 7.5 12.75H16.5C16.91 12.75 17.25 13.09 17.25 13.5C17.25 13.91 16.91 14.25 16.5 14.25Z" fill="{color}"/>
<path d="M9.00028 18.2498C8.85028 18.2498 8.70029 18.2098 8.57029 18.1098C8.23029 17.8698 8.1503 17.3998 8.3903 17.0698L11.2103 13.0698C11.4503 12.7298 11.9203 12.6498 12.2503 12.8898C12.5903 13.1298 12.6703 13.5998 12.4303 13.9298L9.61027 17.9298C9.47027 18.1398 9.23028 18.2498 9.00028 18.2498Z" fill="{color}"/>
<path d="M14.8203 18.2498C14.5803 18.2498 14.3503 18.1398 14.2103 17.9298L11.3903 13.9298C11.1503 13.5898 11.2303 13.1198 11.5703 12.8898C11.9103 12.6498 12.3803 12.7298 12.6103 13.0698L15.4303 17.0698C15.6703 17.4098 15.5903 17.8798 15.2503 18.1098C15.1203 18.2098 14.9703 18.2498 14.8203 18.2498Z" fill="{color}"/>
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<g opacity="0.4">
<path d="M7.5 10.5H16.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9 6.5L11.82 10.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M14.82 6.5L12 10.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7.5 13.5H16.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9 17.5L11.82 13.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M14.82 17.5L12 13.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</g>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
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