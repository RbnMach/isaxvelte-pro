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
<path d="M2 22H22" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9.75 4V22H14.25V4C14.25 2.9 13.8 2 12.45 2H11.55C10.2 2 9.75 2.9 9.75 4Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3 10V22H7V10C7 8.9 6.6 8 5.4 8H4.6C3.4 8 3 8.9 3 10Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17 15V22H21V15C21 13.9 20.6 13 19.4 13H18.6C17.4 13 17 13.9 17 15Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M22 22H2C1.59 22 1.25 21.66 1.25 21.25C1.25 20.84 1.59 20.5 2 20.5H22C22.41 20.5 22.75 20.84 22.75 21.25C22.75 21.66 22.41 22 22 22Z" fill="{color}"/>
<path d="M9.75 4V22H14.25V4C14.25 2.9 13.8 2 12.45 2H11.55C10.2 2 9.75 2.9 9.75 4Z" fill="{color}"/>
<path d="M3 10V22H7V10C7 8.9 6.6 8 5.4 8H4.6C3.4 8 3 8.9 3 10Z" fill="{color}"/>
<path d="M17 15V22H21V15C21 13.9 20.6 13 19.4 13H18.6C17.4 13 17 13.9 17 15Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2 22H22" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9.75 4V22H14.25V4C14.25 2.9 13.8 2 12.45 2H11.55C10.2 2 9.75 2.9 9.75 4Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7 10C7 8.9 6.6 8 5.4 8H4.6C3.4 8 3 8.9 3 10V22H7V13.99" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17 15V22H21V15C21 13.9 20.6 13 19.4 13H18.6C17.4 13 17 13.9 17 15Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M22 22H2C1.59 22 1.25 21.66 1.25 21.25C1.25 20.84 1.59 20.5 2 20.5H22C22.41 20.5 22.75 20.84 22.75 21.25C22.75 21.66 22.41 22 22 22Z" fill="{color}"/>
<path d="M9.75 4V22H14.25V4C14.25 2.9 13.8 2 12.45 2H11.55C10.2 2 9.75 2.9 9.75 4Z" fill="{color}"/>
<path opacity="0.4" d="M3 10V22H7V10C7 8.9 6.6 8 5.4 8H4.6C3.4 8 3 8.9 3 10Z" fill="{color}"/>
<path opacity="0.4" d="M17 15V22H21V15C21 13.9 20.6 13 19.4 13H18.6C17.4 13 17 13.9 17 15Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M21 22.75H3C2.59 22.75 2.25 22.41 2.25 22C2.25 21.59 2.59 21.25 3 21.25H21C21.41 21.25 21.75 21.59 21.75 22C21.75 22.41 21.41 22.75 21 22.75Z" fill="{color}"/>
<path d="M5.59998 19.7499H4C3.04 19.7499 2.25 18.9599 2.25 17.9999V9.37988C2.25 8.41988 3.04 7.62988 4 7.62988H5.59998C6.55998 7.62988 7.34998 8.41988 7.34998 9.37988V17.9999C7.34998 18.9599 6.55998 19.7499 5.59998 19.7499ZM4 9.11987C3.86 9.11987 3.75 9.22987 3.75 9.36987V17.9999C3.75 18.1399 3.86 18.2499 4 18.2499H5.59998C5.73998 18.2499 5.84998 18.1399 5.84998 17.9999V9.37988C5.84998 9.23988 5.73998 9.12988 5.59998 9.12988H4V9.11987Z" fill="{color}"/>
<path d="M12.8002 19.7499H11.2002C10.2402 19.7499 9.4502 18.9599 9.4502 17.9999V6.18994C9.4502 5.22994 10.2402 4.43994 11.2002 4.43994H12.8002C13.7602 4.43994 14.5502 5.22994 14.5502 6.18994V17.9999C14.5502 18.9599 13.7602 19.7499 12.8002 19.7499ZM11.2002 5.93994C11.0602 5.93994 10.9502 6.04994 10.9502 6.18994V17.9999C10.9502 18.1399 11.0602 18.2499 11.2002 18.2499H12.8002C12.9402 18.2499 13.0502 18.1399 13.0502 17.9999V6.18994C13.0502 6.04994 12.9402 5.93994 12.8002 5.93994H11.2002Z" fill="{color}"/>
<path d="M20.0004 19.75H18.4004C17.4404 19.75 16.6504 18.96 16.6504 18V3C16.6504 2.04 17.4404 1.25 18.4004 1.25H20.0004C20.9604 1.25 21.7504 2.04 21.7504 3V18C21.7504 18.96 20.9604 19.75 20.0004 19.75ZM18.4004 2.75C18.2604 2.75 18.1504 2.86 18.1504 3V18C18.1504 18.14 18.2604 18.25 18.4004 18.25H20.0004C20.1404 18.25 20.2504 18.14 20.2504 18V3C20.2504 2.86 20.1404 2.75 20.0004 2.75H18.4004Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2 22H22" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9.75 4V22H14.25V4C14.25 2.9 13.8 2 12.45 2H11.55C10.2 2 9.75 2.9 9.75 4Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M3 10V22H7V10C7 8.9 6.6 8 5.4 8H4.6C3.4 8 3 8.9 3 10Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M17 15V22H21V15C21 13.9 20.6 13 19.4 13H18.6C17.4 13 17 13.9 17 15Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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