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
<path d="M7.0999 3.5H15.9999C19.9999 3.5 21.9999 6 21.9999 9.5V12C21.9999 17 18.9999 20.5 13.4999 20.5H3.8999L4.9999 16.2H12.3999C15.9999 16.2 17.6999 14 17.6999 10.9V10.7C17.6999 8.9 16.8999 7.7 14.6999 7.7H6.0999L7.0999 3.5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.5 10.5H4.3C3.4 10.5 2.6 11.1 2.4 12L2 13.5H9.2C10.1 13.5 10.9 12.9 11.1 12L11.5 10.5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M7.11945 3.5H15.9995C19.9995 3.5 21.9995 6 21.9995 9.5V12C21.9995 17 18.9995 20.5 13.4995 20.5H3.93945L4.99945 16.25H12.4395C15.9995 16.25 17.7495 14 17.7495 10.94V10.75C17.7495 9 16.9995 7.75 14.7495 7.75H6.05945L7.11945 3.5Z" fill="{color}"/>
<path d="M12.4095 10.2305H4.69952C3.61952 10.2305 2.67952 10.9705 2.40952 12.0105L2.15952 13.0305C2.06952 13.4005 2.34952 13.7605 2.72952 13.7605H10.4395C11.5195 13.7605 12.4595 13.0205 12.7295 11.9805L12.9795 10.9605C13.0795 10.5905 12.7895 10.2305 12.4095 10.2305Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M6.00945 20.5H3.93945L4.99945 16.25H12.4395C15.9995 16.25 17.7495 14 17.7495 10.94V10.75C17.7495 9 16.9995 7.75 14.7495 7.75H6.05945L7.11945 3.5H15.9995C19.9995 3.5 21.9995 6 21.9995 9.5V12C21.9995 17 18.9995 20.5 13.4995 20.5H10.9395" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.5 10.5H4.31C3.39 10.5 2.59 11.12 2.37 12.01L2 13.5H9.19C10.11 13.5 10.91 12.88 11.13 11.99L11.5 10.5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M9.493 4.667h11.84c5.333 0 8 3.333 8 8v3.333c0 6.667-4 11.333-11.333 11.333h-12.747l1.413-5.667h9.92c4.747 0 7.080-3 7.080-7.080v-0.253c0-2.333-1-4-4-4h-11.587l1.413-5.667z"></path>
<path fill="{color}" d="M16.546 13.64h-10.28c-1.44 0-2.693 0.987-3.053 2.373l-0.333 1.36c-0.12 0.493 0.253 0.973 0.76 0.973h10.28c1.44 0 2.693-0.987 3.053-2.373l0.333-1.36c0.133-0.493-0.253-0.973-0.76-0.973z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M13.5003 21.25H3.94032C3.71032 21.25 3.49032 21.14 3.35032 20.96C3.21032 20.78 3.16032 20.54 3.21032 20.32L4.27032 16.07C4.35032 15.74 4.65032 15.5 5.00032 15.5H12.4403C15.3403 15.5 17.0003 13.84 17.0003 10.94V10.75C17.0003 9.15 16.3503 8.5 14.7503 8.5H6.06032C5.83032 8.5 5.61032 8.39001 5.47032 8.21001C5.33032 8.03001 5.28032 7.79001 5.33032 7.57001L6.39032 3.32001C6.47032 2.99001 6.77032 2.75 7.12032 2.75H16.0003C20.1603 2.75 22.7503 5.34 22.7503 9.5V12C22.7503 17.71 19.2103 21.25 13.5003 21.25ZM4.90032 19.75H13.5003C18.3503 19.75 21.2503 16.85 21.2503 12V9.5C21.2503 6.16 19.3403 4.25 16.0003 4.25H7.71032L7.02032 7H14.7503C17.1703 7 18.5003 8.33 18.5003 10.75V10.94C18.5003 14.68 16.1803 17 12.4403 17H5.59032L4.90032 19.75Z" fill="{color}"/>
<path d="M9.18989 14.2498H1.99989C1.76989 14.2498 1.54989 14.1398 1.40989 13.9598C1.26989 13.7798 1.21989 13.5398 1.26989 13.3198L1.63989 11.8398C1.94989 10.6098 3.03989 9.75977 4.30989 9.75977H11.4999C11.7299 9.75977 11.9499 9.86977 12.0899 10.0498C12.2299 10.2298 12.2799 10.4698 12.2299 10.6898L11.8599 12.1698C11.5499 13.3898 10.4499 14.2498 9.18989 14.2498ZM2.95989 12.7498H9.18989C9.75989 12.7498 10.2599 12.3598 10.3999 11.7998L10.5399 11.2498H4.30989C3.73989 11.2498 3.23989 11.6398 3.09989 12.1998L2.95989 12.7498Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M7.12043 3.5H16.0004C20.0004 3.5 22.0004 6 22.0004 9.5V12C22.0004 17 19.0004 20.5 13.5004 20.5H3.94043L5.00043 16.25H12.4404C16.0004 16.25 17.7504 14 17.7504 10.94V10.75C17.7504 9 17.0004 7.75 14.7504 7.75H6.06043L7.12043 3.5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M11.5 10.5H4.31C3.39 10.5 2.59 11.12 2.37 12.01L2 13.5H9.19C10.11 13.5 10.91 12.88 11.13 11.99L11.5 10.5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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