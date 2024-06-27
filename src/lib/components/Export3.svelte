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
<path d="M13 11L21.2 2.80005" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M22 6.8V2H17.2" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11 2H9C4 2 2 4 2 9V15C2 20 4 22 9 22H15C20 22 22 20 22 15V13" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.19 2H7.81C4.17 2 2 4.17 2 7.81V16.18C2 19.83 4.17 22 7.81 22H16.18C19.82 22 21.99 19.83 21.99 16.19V7.81C22 4.17 19.83 2 16.19 2ZM17.25 12.33C17.25 12.74 16.91 13.08 16.5 13.08C16.09 13.08 15.75 12.74 15.75 12.33V9.31L8.03 17.03C7.88 17.18 7.69 17.25 7.5 17.25C7.31 17.25 7.12 17.18 6.97 17.03C6.68 16.74 6.68 16.26 6.97 15.97L14.69 8.25H11.67C11.26 8.25 10.92 7.91 10.92 7.5C10.92 7.09 11.26 6.75 11.67 6.75H16.5C16.91 6.75 17.25 7.09 17.25 7.5V12.33Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M13 11L21.2 2.80005" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M21.9992 6.8V2H17.1992" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 12.99V15C2 20 4 22 9 22H15C20 22 22 20 22 15V13" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11 2H9C4 2 2 4 2 9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M16.19 2H7.81C4.17 2 2 4.17 2 7.81V16.18C2 19.83 4.17 22 7.81 22H16.18C19.82 22 21.99 19.83 21.99 16.19V7.81C22 4.17 19.83 2 16.19 2Z" fill="{color}"/>
<path d="M16.7475 7H11.9175C11.5075 7 11.1675 7.34 11.1675 7.75C11.1675 8.16 11.5075 8.5 11.9175 8.5H14.9375L7.2175 16.22C6.9275 16.51 6.9275 16.99 7.2175 17.28C7.3675 17.43 7.5575 17.5 7.7475 17.5C7.9375 17.5 8.1275 17.43 8.2775 17.28L15.9975 9.56V12.58C15.9975 12.99 16.3375 13.33 16.7475 13.33C17.1575 13.33 17.4975 12.99 17.4975 12.58V7.75C17.4975 7.34 17.1575 7 16.7475 7Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12.9995 11.75C12.8095 11.75 12.6195 11.68 12.4695 11.53C12.1795 11.24 12.1795 10.76 12.4695 10.47L20.6695 2.26999C20.9595 1.97999 21.4395 1.97999 21.7295 2.26999C22.0195 2.55999 22.0195 3.03999 21.7295 3.32999L13.5295 11.53C13.3795 11.68 13.1895 11.75 12.9995 11.75Z" fill="{color}"/>
<path d="M21.9992 7.55C21.5892 7.55 21.2492 7.21 21.2492 6.8V2.75H17.1992C16.7892 2.75 16.4492 2.41 16.4492 2C16.4492 1.59 16.7892 1.25 17.1992 1.25H21.9992C22.4092 1.25 22.7492 1.59 22.7492 2V6.8C22.7492 7.21 22.4092 7.55 21.9992 7.55Z" fill="{color}"/>
<path d="M15 22.75H9C3.57 22.75 1.25 20.43 1.25 15V9C1.25 3.57 3.57 1.25 9 1.25H11C11.41 1.25 11.75 1.59 11.75 2C11.75 2.41 11.41 2.75 11 2.75H9C4.39 2.75 2.75 4.39 2.75 9V15C2.75 19.61 4.39 21.25 9 21.25H15C19.61 21.25 21.25 19.61 21.25 15V13C21.25 12.59 21.59 12.25 22 12.25C22.41 12.25 22.75 12.59 22.75 13V15C22.75 20.43 20.43 22.75 15 22.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<g opacity="0.4">
<path d="M13 10.9998L21.2 2.7998" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M21.9992 6.8V2H17.1992" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</g>
<path d="M11 2H9C4 2 2 4 2 9V15C2 20 4 22 9 22H15C20 22 22 20 22 15V13" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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