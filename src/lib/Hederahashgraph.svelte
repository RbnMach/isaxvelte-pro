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
<path d="M8.2002 16.5V7.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.7998 16.5V7.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.2002 10.1001H15.8002" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.2002 13.8999H15.8002" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15 10.8789H9V13.1289H15V10.8789Z" fill="{color}"/>
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM16.5 16.5C16.5 16.91 16.16 17.25 15.75 17.25C15.34 17.25 15 16.91 15 16.5V14.62H9V16.5C9 16.91 8.66 17.25 8.25 17.25C7.84 17.25 7.5 16.91 7.5 16.5V7.5C7.5 7.09 7.84 6.75 8.25 6.75C8.66 6.75 9 7.09 9 7.5V9.38H15V7.5C15 7.09 15.34 6.75 15.75 6.75C16.16 6.75 16.5 7.09 16.5 7.5V16.5Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M8.25 16.5V7.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.75 16.5V7.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.25 10.1299H15.75" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.25 13.8701H15.75" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.19997 2.3 7.96997 2.85" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="none" stroke="{color}" stroke-linejoin="round" stroke-linecap="round" stroke-miterlimit="10" stroke-width="2" d="M10 23.2v-14.4"></path>
<path fill="none" stroke="{color}" stroke-linejoin="round" stroke-linecap="round" stroke-miterlimit="10" stroke-width="2" d="M10 13.008h12"></path>
<path fill="{color}" opacity="0.4" d="M16 32c8.837 0 16-7.163 16-16s-7.163-16-16-16c-8.837 0-16 7.163-16 16s7.163 16 16 16z"></path>
<path fill="{color}" d="M21.999 24.4c-0.656 0-1.2-0.544-1.2-1.2v-14.4c0-0.656 0.544-1.2 1.2-1.2s1.2 0.544 1.2 1.2v14.4c0 0.656-0.544 1.2-1.2 1.2z"></path>
<path fill="{color}" d="M22 20.192h-12c-0.656 0 0.133-0.544 0.133-1.2s-0.789-1.2-0.133-1.2h12c0.656 0 1.2 0.544 1.2 1.2s-0.544 1.2-1.2 1.2z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M8.25 17.25C7.84 17.25 7.5 16.91 7.5 16.5V7.5C7.5 7.09 7.84 6.75 8.25 6.75C8.66 6.75 9 7.09 9 7.5V16.5C9 16.91 8.66 17.25 8.25 17.25Z" fill="{color}"/>
<path d="M15.75 17.25C15.34 17.25 15 16.91 15 16.5V7.5C15 7.09 15.34 6.75 15.75 6.75C16.16 6.75 16.5 7.09 16.5 7.5V16.5C16.5 16.91 16.16 17.25 15.75 17.25Z" fill="{color}"/>
<path d="M15.75 10.8799H8.25C7.84 10.8799 7.5 10.5399 7.5 10.1299C7.5 9.71988 7.84 9.37988 8.25 9.37988H15.75C16.16 9.37988 16.5 9.71988 16.5 10.1299C16.5 10.5399 16.16 10.8799 15.75 10.8799Z" fill="{color}"/>
<path d="M15.75 14.6201H8.25C7.84 14.6201 7.5 14.2801 7.5 13.8701C7.5 13.4601 7.84 13.1201 8.25 13.1201H15.75C16.16 13.1201 16.5 13.4601 16.5 13.8701C16.5 14.2801 16.16 14.6201 15.75 14.6201Z" fill="{color}"/>
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<g opacity="0.4">
<path d="M8.25 16.5V7.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.75 16.5V7.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.25 10.1299H15.75" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.25 13.8701H15.75" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</g>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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