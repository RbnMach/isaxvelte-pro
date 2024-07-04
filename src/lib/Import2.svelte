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
<path d="M9.31995 11.6799L11.8799 14.2399L14.4399 11.6799" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.88 4V14.17" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M20 12.1799C20 16.5999 17 20.1799 12 20.1799C7 20.1799 4 16.5999 4 12.1799" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M21.14 9.89844H12.68V13.5684L14.25 11.9984C14.54 11.7084 15.02 11.7084 15.31 11.9984C15.6 12.2884 15.6 12.7684 15.31 13.0584L12.46 15.8984C12.17 16.1884 11.69 16.1884 11.4 15.8984L8.55 13.0584C8.4 12.9084 8.33 12.7184 8.33 12.5284C8.33 12.3384 8.41 12.1484 8.56 11.9984C8.85 11.7084 9.33 11.7084 9.62 11.9984L11.18 13.5584V9.89844H2.86C2.38 9.89844 2 10.2784 2 10.7584C2 16.6484 6.11 20.7584 12 20.7584C17.89 20.7584 22 16.6484 22 10.7584C22 10.2784 21.62 9.89844 21.14 9.89844Z" fill="{color}"/>
<path d="M12.6797 3.98828C12.6797 3.57828 12.3397 3.23828 11.9297 3.23828C11.5197 3.23828 11.1797 3.57828 11.1797 3.98828V9.88828H12.6797V3.98828Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M9.43945 11.6799L11.9995 14.2399L14.5595 11.6799" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 9V14.17" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 4V5.96" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17.52 18.01C16.16 19.25 14.29 20 12 20C7 20 4 16.42 4 12" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M19.9998 12C19.9998 13.05 19.8298 14.05 19.5098 14.97" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M22 10.7599C22 10.2899 21.62 9.8999 21.14 9.8999H2.86C2.38 9.8999 2 10.2799 2 10.7599C2 16.6499 6.11 20.7599 12 20.7599C17.89 20.7599 22 16.6399 22 10.7599Z" fill="{color}"/>
<path d="M12.4598 15.9L15.3098 13.06C15.5998 12.77 15.5998 12.29 15.3098 12C15.0198 11.71 14.5398 11.71 14.2498 12L12.6898 13.56V3.98999C12.6898 3.57999 12.3498 3.23999 11.9398 3.23999C11.5298 3.23999 11.1898 3.57999 11.1898 3.98999V13.56L9.61984 12C9.32984 11.71 8.84984 11.71 8.55984 12C8.40984 12.15 8.33984 12.34 8.33984 12.53C8.33984 12.72 8.40984 12.91 8.55984 13.06L11.4098 15.9C11.6998 16.2 12.1698 16.2 12.4598 15.9Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11.8798 14.9901C11.6898 14.9901 11.4998 14.9201 11.3498 14.7701L8.78977 12.2101C8.49977 11.9201 8.49977 11.4401 8.78977 11.1501C9.07977 10.8601 9.55977 10.8601 9.84977 11.1501L11.8798 13.1801L13.9098 11.1501C14.1998 10.8601 14.6798 10.8601 14.9698 11.1501C15.2598 11.4401 15.2598 11.9201 14.9698 12.2101L12.4098 14.7701C12.2598 14.9201 12.0698 14.9901 11.8798 14.9901Z" fill="{color}"/>
<path d="M11.8809 14.92C11.4709 14.92 11.1309 14.58 11.1309 14.17V4C11.1309 3.59 11.4709 3.25 11.8809 3.25C12.2909 3.25 12.6309 3.59 12.6309 4V14.17C12.6309 14.58 12.2909 14.92 11.8809 14.92Z" fill="{color}"/>
<path d="M12 20.9299C6.85 20.9299 3.25 17.3299 3.25 12.1799C3.25 11.7699 3.59 11.4299 4 11.4299C4.41 11.4299 4.75 11.7699 4.75 12.1799C4.75 16.4499 7.73 19.4299 12 19.4299C16.27 19.4299 19.25 16.4499 19.25 12.1799C19.25 11.7699 19.59 11.4299 20 11.4299C20.41 11.4299 20.75 11.7699 20.75 12.1799C20.75 17.3299 17.15 20.9299 12 20.9299Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<g opacity="0.4">
<path d="M9.32031 11.6797L11.8803 14.2397L14.4403 11.6797" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.8809 4V14.17" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</g>
<path d="M20 12.1802C20 16.6002 17 20.1802 12 20.1802C7 20.1802 4 16.6002 4 12.1802" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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