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
<path d="M11 18V21C11 21.5 10.6 22 10 22C9.4 22 9 21.5 9 21V18H11Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15 18V21C15 21.5 14.6 22 14 22C13.4 22 13 21.5 13 21V18H15Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17 11V16C17 17.1 16.1 18 15 18H9C7.9 18 7 17.1 7 16V11C7 9.9 7.9 9 9 9H15C16.1 9 17 9.9 17 11Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5 11V15C5 15.6 4.6 16 4 16C3.4 16 3 15.6 3 15V11C3 10.4 3.4 10 4 10C4.6 10 5 10.4 5 11Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M21 11V15C21 15.6 20.6 16 20 16C19.4 16 19 15.6 19 15V11C19 10.4 19.4 10 20 10C20.6 10 21 10.4 21 11Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M13 18H11" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9.6 7H14.4C15.3 7 16 6.25 16 5.28571C16 2.92857 14.2 1 12 1C9.8 1 8 2.92857 8 5.28571C8 6.25 8.7 7 9.6 7Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11 18V21C11 21.55 10.55 22 10 22C9.45 22 9 21.55 9 21V18H11Z" fill="{color}"/>
<path d="M15 18V21C15 21.55 14.55 22 14 22C13.45 22 13 21.55 13 21V18H15Z" fill="{color}"/>
<path d="M17 11V16C17 17.1 16.1 18 15 18H9C7.9 18 7 17.1 7 16V11C7 9.9 7.9 9 9 9H15C16.1 9 17 9.9 17 11Z" fill="{color}"/>
<path d="M5 11V15C5 15.55 4.55 16 4 16C3.45 16 3 15.55 3 15V11C3 10.45 3.45 10 4 10C4.55 10 5 10.45 5 11Z" fill="{color}"/>
<path d="M21 11V15C21 15.55 20.55 16 20 16C19.45 16 19 15.55 19 15V11C19 10.45 19.45 10 20 10C20.55 10 21 10.45 21 11Z" fill="{color}"/>
<path d="M9.59998 7.60001H14.4C15.28 7.60001 16 6.88 16 6C16 3.79 14.21 2 12 2C9.79 2 8 3.79 8 6C8 6.88 8.71998 7.60001 9.59998 7.60001Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11 18V21C11 21.55 10.55 22 10 22C9.45 22 9 21.55 9 21V18H11Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15 18V21C15 21.55 14.55 22 14 22C13.45 22 13 21.55 13 21V18H15Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7 11C7 9.9 7.9 9 9 9H15C16.1 9 17 9.9 17 11V16C17 17.1 16.1 18 15 18H9C7.9 18 7 17.1 7 16V15.29" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5 11V15C5 15.55 4.55 16 4 16C3.45 16 3 15.55 3 15V11C3 10.45 3.45 10 4 10C4.55 10 5 10.45 5 11Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M21 11V15C21 15.55 20.55 16 20 16C19.45 16 19 15.55 19 15V11C19 10.45 19.45 10 20 10C20.55 10 21 10.45 21 11Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M13 18H11" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9.59998 6.99991H14.4C15.28 6.99991 16 6.2799 16 5.3999C16 3.1899 14.21 1.3999 12 1.3999C9.79 1.3999 8 3.1899 8 5.3999C8 6.2799 8.71998 6.99991 9.59998 6.99991Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" d="M14.667 24v4c0 0.733-0.6 1.333-1.333 1.333s-1.333-0.6-1.333-1.333v-4h2.667z"></path>
<path fill="{color}" d="M20 24v4c0 0.733-0.6 1.333-1.333 1.333s-1.333-0.6-1.333-1.333v-4h2.667z"></path>
<path fill="{color}" opacity="0.4" d="M22.667 14.667v6.667c0 1.467-1.2 2.667-2.667 2.667h-8c-1.467 0-2.667-1.2-2.667-2.667v-6.667c0-1.467 1.2-2.667 2.667-2.667h8c1.467 0 2.667 1.2 2.667 2.667z"></path>
<path fill="{color}" d="M6.667 14.667v5.333c0 0.733-0.6 1.333-1.333 1.333s-1.333-0.6-1.333-1.333v-5.333c0-0.733 0.6-1.333 1.333-1.333s1.333 0.6 1.333 1.333z"></path>
<path fill="{color}" d="M28 14.667v5.333c0 0.733-0.6 1.333-1.333 1.333s-1.333-0.6-1.333-1.333v-5.333c0-0.733 0.6-1.333 1.333-1.333s1.333 0.6 1.333 1.333z"></path>
<path fill="{color}" opacity="0.4" d="M12.8 10.133h6.4c1.173 0 2.133-0.96 2.133-2.133 0-2.947-2.387-5.333-5.333-5.333s-5.333 2.387-5.333 5.333c0 1.173 0.96 2.133 2.133 2.133z"></path>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M10 22.75C9.04 22.75 8.25 21.96 8.25 21V18C8.25 17.59 8.59 17.25 9 17.25H11C11.41 17.25 11.75 17.59 11.75 18V21C11.75 21.96 10.96 22.75 10 22.75ZM9.75 18.75V21C9.75 21.27 10.25 21.27 10.25 21V18.75H9.75Z" fill="{color}"/>
<path d="M14 22.75C13.04 22.75 12.25 21.96 12.25 21V18C12.25 17.59 12.59 17.25 13 17.25H15C15.41 17.25 15.75 17.59 15.75 18V21C15.75 21.96 14.96 22.75 14 22.75ZM13.75 18.75V21C13.75 21.27 14.25 21.27 14.25 21V18.75H13.75Z" fill="{color}"/>
<path d="M15 18.75H9C7.48 18.75 6.25 17.52 6.25 16V11C6.25 9.48 7.48 8.25 9 8.25H15C16.52 8.25 17.75 9.48 17.75 11V16C17.75 17.52 16.52 18.75 15 18.75ZM9 9.75C8.31 9.75 7.75 10.31 7.75 11V16C7.75 16.69 8.31 17.25 9 17.25H15C15.69 17.25 16.25 16.69 16.25 16V11C16.25 10.31 15.69 9.75 15 9.75H9Z" fill="{color}"/>
<path d="M4 16.75C3.04 16.75 2.25 15.96 2.25 15V11C2.25 10.04 3.04 9.25 4 9.25C4.96 9.25 5.75 10.04 5.75 11V15C5.75 15.96 4.96 16.75 4 16.75ZM4 10.75C3.86 10.75 3.75 10.86 3.75 11V15C3.75 15.28 4.25 15.28 4.25 15V11C4.25 10.86 4.14 10.75 4 10.75Z" fill="{color}"/>
<path d="M20 16.75C19.04 16.75 18.25 15.96 18.25 15V11C18.25 10.04 19.04 9.25 20 9.25C20.96 9.25 21.75 10.04 21.75 11V15C21.75 15.96 20.96 16.75 20 16.75ZM20 10.75C19.86 10.75 19.75 10.86 19.75 11V15C19.75 15.28 20.25 15.28 20.25 15V11C20.25 10.86 20.14 10.75 20 10.75Z" fill="{color}"/>
<path d="M13 18.75H11C10.59 18.75 10.25 18.41 10.25 18C10.25 17.59 10.59 17.25 11 17.25H13C13.41 17.25 13.75 17.59 13.75 18C13.75 18.41 13.41 18.75 13 18.75Z" fill="{color}"/>
<path d="M14.4 7.74991H9.59998C8.29998 7.74991 7.25 6.6999 7.25 5.3999C7.25 2.7799 9.38 0.649902 12 0.649902C14.62 0.649902 16.75 2.7799 16.75 5.3999C16.75 6.6999 15.7 7.74991 14.4 7.74991ZM12 2.1499C10.21 2.1499 8.75 3.6099 8.75 5.3999C8.75 5.8699 9.12998 6.24991 9.59998 6.24991H14.4C14.87 6.24991 15.25 5.8699 15.25 5.3999C15.25 3.6099 13.79 2.1499 12 2.1499Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11 18V21C11 21.55 10.55 22 10 22C9.45 22 9 21.55 9 21V18H11Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15 18V21C15 21.55 14.55 22 14 22C13.45 22 13 21.55 13 21V18H15Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17 11V16C17 17.1 16.1 18 15 18H9C7.9 18 7 17.1 7 16V11C7 9.9 7.9 9 9 9H15C16.1 9 17 9.9 17 11Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M5 11V15C5 15.55 4.55 16 4 16C3.45 16 3 15.55 3 15V11C3 10.45 3.45 10 4 10C4.55 10 5 10.45 5 11Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M21 11V15C21 15.55 20.55 16 20 16C19.45 16 19 15.55 19 15V11C19 10.45 19.45 10 20 10C20.55 10 21 10.45 21 11Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M13 18H11" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M9.59998 6.99991H14.4C15.28 6.99991 16 6.2799 16 5.3999C16 3.1899 14.21 1.3999 12 1.3999C9.79 1.3999 8 3.1899 8 5.3999C8 6.2799 8.71998 6.99991 9.59998 6.99991Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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