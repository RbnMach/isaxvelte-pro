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
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path d="M11.9999 5.8999L9.3999 10.0999H14.5999L11.9999 5.8999Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.6 11.8999L6 16.0999H11.1L8.6 11.8999Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.3999 11.8999L12.8999 16.0999H17.9999L15.3999 11.8999Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM10.7 16.14H6.44C6.25 16.14 6.12998 15.93 6.22998 15.76L8.35999 12.21C8.45999 12.05 8.68998 12.05 8.78998 12.21L10.92 15.76C11.02 15.93 10.9 16.14 10.7 16.14ZM9.87 10.14C9.68 10.14 9.55997 9.92999 9.65997 9.75999L11.79 6.21001C11.89 6.05001 12.12 6.05001 12.22 6.21001L14.35 9.75999C14.45 9.92999 14.33 10.14 14.14 10.14H9.87ZM17.56 16.14H13.3C13.11 16.14 12.99 15.93 13.09 15.76L15.22 12.21C15.32 12.05 15.55 12.05 15.65 12.21L17.78 15.76C17.87 15.93 17.75 16.14 17.56 16.14Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11.9997 5.86011L9.42969 10.1401H14.5697L11.9997 5.86011Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.57001 11.8601L6 16.1401H11.14L8.57001 11.8601Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.4294 11.8601L12.8594 16.1401H17.9994L15.4294 11.8601Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.19997 2.30001 7.96997 2.85001" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M15.72 8.28l-2.84 4.733c-0.133 0.227 0.027 0.507 0.28 0.507h5.68c0.253 0 0.413-0.28 0.28-0.507l-2.84-4.733c-0.12-0.213-0.44-0.213-0.56 0z"></path>
<path fill="{color}" d="M11.146 16.28l-2.84 4.733c-0.133 0.227 0.027 0.507 0.28 0.507h5.68c0.253 0 0.413-0.28 0.28-0.507l-2.84-4.733c-0.12-0.213-0.44-0.213-0.56 0z"></path>
<path fill="{color}" d="M20.28 16.28l-2.84 4.733c-0.133 0.227 0.027 0.507 0.28 0.507h5.68c0.253 0 0.413-0.28 0.28-0.507l-2.84-4.733c-0.107-0.213-0.427-0.213-0.56 0z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
<path d="M14.5699 10.8901H9.42987C9.15987 10.8901 8.9099 10.74 8.7799 10.51C8.6499 10.27 8.64985 9.99005 8.78985 9.75005L11.3599 5.46006C11.6299 5.01006 12.3799 5.01006 12.6499 5.46006L15.2198 9.75005C15.3598 9.98005 15.3599 10.27 15.2299 10.51C15.0899 10.75 14.8399 10.8901 14.5699 10.8901ZM10.7499 9.39005H13.2399L11.9899 7.31005L10.7499 9.39005Z" fill="{color}"/>
<path d="M11.1402 16.8898H6.00021C5.73021 16.8898 5.48019 16.7398 5.35019 16.5098C5.22019 16.2798 5.2202 15.9898 5.3602 15.7598L7.9302 11.4698C8.2002 11.0198 8.95018 11.0198 9.22018 11.4698L11.7902 15.7598C11.9302 15.9898 11.9302 16.2798 11.8002 16.5098C11.6602 16.7498 11.4102 16.8898 11.1402 16.8898ZM7.32022 15.3898H9.81021L8.56021 13.3098L7.32022 15.3898Z" fill="{color}"/>
<path d="M17.9996 16.8898H12.8596C12.5896 16.8898 12.3396 16.7398 12.2096 16.5098C12.0796 16.2798 12.0795 15.9898 12.2195 15.7598L14.7895 11.4698C15.0595 11.0198 15.8096 11.0198 16.0796 11.4698L18.6496 15.7598C18.7896 15.9898 18.7895 16.2798 18.6595 16.5098C18.5195 16.7498 18.2696 16.8898 17.9996 16.8898ZM14.1796 15.3898H16.6696L15.4196 13.3098L14.1796 15.3898Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path opacity="0.4" d="M11.9997 5.85986L9.42969 10.1399H14.5697L11.9997 5.85986Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M8.57001 11.8599L6 16.1399H11.14L8.57001 11.8599Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M15.4304 11.8599L12.8604 16.1399H18.0004L15.4304 11.8599Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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