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
<path d="M2 3H22" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3.99988 6.3999H19.9999C20.8999 6.3999 21.3999 7.3999 20.8999 8.0999L12.8999 20.4999C12.4999 21.1999 11.4999 21.1999 10.9999 20.4999L2.99988 8.0999C2.59988 7.2999 3.19988 6.3999 3.99988 6.3999Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M21 3.14844H3C2.59 3.14844 2.25 3.48844 2.25 3.89844C2.25 4.30844 2.59 4.64844 3 4.64844H21C21.41 4.64844 21.75 4.30844 21.75 3.89844C21.75 3.48844 21.41 3.14844 21 3.14844Z" fill="{color}"/>
<path d="M4.04088 6.23828H19.9709C20.8509 6.23828 21.3809 7.20828 20.9009 7.94828L12.9409 20.3383C12.5009 21.0183 11.5109 21.0183 11.0709 20.3383L3.11086 7.94828C2.63086 7.20828 3.16088 6.23828 4.04088 6.23828Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2 3.03003H22" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3.69939 9.00011L3.10937 8.07011C2.62937 7.33011 3.16939 6.36011 4.03939 6.36011H19.9694C20.8494 6.36011 21.3794 7.33011 20.8994 8.07011L12.9394 20.4601C12.4994 21.1401 11.5094 21.1401 11.0694 20.4601L5.80938 12.2801" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" d="M28 4.2h-24c-0.547 0-1 0.453-1 1s0.453 1 1 1h24c0.547 0 1-0.453 1-1s-0.453-1-1-1z"></path>
<path fill="{color}" d="M5.385 8.32h21.24c1.173 0 1.88 1.293 1.24 2.28l-10.613 16.52c-0.587 0.907-1.907 0.907-2.493 0l-10.627-16.52c-0.627-0.987 0.080-2.28 1.253-2.28z"></path>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M22 3.77979H2C1.59 3.77979 1.25 3.43979 1.25 3.02979C1.25 2.61979 1.59 2.27979 2 2.27979H22C22.41 2.27979 22.75 2.61979 22.75 3.02979C22.75 3.43979 22.41 3.77979 22 3.77979Z" fill="{color}"/>
<path d="M11.9997 21.7199C11.3597 21.7199 10.7797 21.3999 10.4297 20.8699L2.46966 8.47987C2.09966 7.90987 2.07965 7.17986 2.39965 6.57986C2.72965 5.97986 3.34966 5.60986 4.02966 5.60986H19.9597C20.6397 5.60986 21.2697 5.97986 21.5897 6.57986C21.9197 7.17986 21.8896 7.90987 21.5196 8.47987L13.5597 20.8699C13.2197 21.3999 12.6397 21.7199 11.9997 21.7199ZM4.03967 7.10986C3.84967 7.10986 3.74966 7.23987 3.71966 7.29987C3.68966 7.35987 3.62967 7.50986 3.72967 7.66986L11.6897 20.0599C11.7797 20.1999 11.9196 20.2299 11.9896 20.2299C12.0596 20.2299 12.1997 20.2099 12.2897 20.0599L20.2497 7.66986C20.3497 7.50986 20.2897 7.35987 20.2597 7.29987C20.2297 7.23987 20.1397 7.10986 19.9397 7.10986H4.03967Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2 3.02979H22" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M4.0399 6.35986H19.9699C20.8499 6.35986 21.3799 7.32986 20.8999 8.06986L12.9399 20.4599C12.4999 21.1399 11.5099 21.1399 11.0699 20.4599L3.10988 8.06986C2.62988 7.32986 3.1599 6.35986 4.0399 6.35986Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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