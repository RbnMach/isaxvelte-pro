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
<path d="M15.1 18H8.9C7.9 18 7 17.2 7 16.1V7.9C7 6.8 7.8 6 8.9 6H15.2C16.2 6 17.1 6.8 17.1 7.9V16.2C17 17.2 16.2 18 15.1 18Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 8.5V10.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10 10.5H14" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 15.5V13.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10 13.5H14" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15 22H9C4 22 2 20 2 15V9C2 4 4 2 9 2H15C20 2 22 4 22 9V15C22 20 20 22 15 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M14 9.75H12.75V8.5C12.75 8.09 12.41 7.75 12 7.75C11.59 7.75 11.25 8.09 11.25 8.5V9.75H10C9.59 9.75 9.25 10.09 9.25 10.5C9.25 10.91 9.59 11.25 10 11.25H14C14.41 11.25 14.75 10.91 14.75 10.5C14.75 10.09 14.41 9.75 14 9.75Z" fill="{color}"/>
<path d="M14 12.75H10C9.59 12.75 9.25 13.09 9.25 13.5C9.25 13.91 9.59 14.25 10 14.25H11.25V15.5C11.25 15.91 11.59 16.25 12 16.25C12.41 16.25 12.75 15.91 12.75 15.5V14.25H14C14.41 14.25 14.75 13.91 14.75 13.5C14.75 13.09 14.41 12.75 14 12.75Z" fill="{color}"/>
<path d="M16.1898 2H7.81976C4.17976 2 2.00977 4.17 2.00977 7.81V16.18C2.00977 19.82 4.17976 21.99 7.81976 21.99H16.1898C19.8298 21.99 21.9998 19.82 21.9998 16.18V7.81C21.9998 4.17 19.8298 2 16.1898 2ZM16.9998 16.15C16.9998 17.17 16.1698 18 15.1498 18H8.84973C7.82973 18 6.99976 17.17 6.99976 16.15V7.85C6.99976 6.83 7.82973 6 8.84973 6H15.1498C16.1698 6 16.9998 6.83 16.9998 7.85V16.15Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15.15 18H8.84998C7.82998 18 7 17.17 7 16.15V7.85C7 6.83 7.82998 6 8.84998 6H15.15C16.17 6 17 6.83 17 7.85V16.15C17 17.17 16.17 18 15.15 18Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 8.5V10.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10 10.5H14" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 15.5V13.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10 13.5H14" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 12.83V15C2 20 4 22 9 22H15C20 22 22 20 22 15V9C22 4 20 2 15 2H9C4 2 2 4 2 9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M21.587 2.667h-11.16c-4.867 0-7.76 2.893-7.76 7.747v11.16c0 4.853 2.893 7.747 7.747 7.747h11.16c4.853 0 7.747-2.893 7.747-7.747v-11.16c0.013-4.853-2.88-7.747-7.733-7.747z"></path>
<path fill="{color}" d="M20.2 8h-8.4c-1.36 0-2.467 1.107-2.467 2.467v11.067c0 1.36 1.107 2.467 2.467 2.467h8.4c1.36 0 2.467-1.107 2.467-2.467v-11.067c0-1.36-1.107-2.467-2.467-2.467zM18.667 19h-1.667v1.667c0 0.547-0.453 1-1 1s-1-0.453-1-1v-1.667h-1.667c-0.547 0-1-0.453-1-1s0.453-1 1-1h5.333c0.547 0 1 0.453 1 1s-0.453 1-1 1zM18.667 15h-5.333c-0.547 0-1-0.453-1-1s0.453-1 1-1h1.667v-1.667c0-0.547 0.453-1 1-1s1 0.453 1 1v1.667h1.667c0.547 0 1 0.453 1 1s-0.453 1-1 1z"></path>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15.15 18.75H8.84998C7.41998 18.75 6.25 17.58 6.25 16.15V7.85C6.25 6.42 7.41998 5.25 8.84998 5.25H15.15C16.58 5.25 17.75 6.42 17.75 7.85V16.15C17.75 17.58 16.58 18.75 15.15 18.75ZM8.84998 6.75C8.23998 6.75 7.75 7.24 7.75 7.85V16.15C7.75 16.76 8.23998 17.25 8.84998 17.25H15.15C15.76 17.25 16.25 16.76 16.25 16.15V7.85C16.25 7.24 15.76 6.75 15.15 6.75H8.84998Z" fill="{color}"/>
<path d="M12 11.25C11.59 11.25 11.25 10.91 11.25 10.5V8.5C11.25 8.09 11.59 7.75 12 7.75C12.41 7.75 12.75 8.09 12.75 8.5V10.5C12.75 10.91 12.41 11.25 12 11.25Z" fill="{color}"/>
<path d="M14 11.25H10C9.59 11.25 9.25 10.91 9.25 10.5C9.25 10.09 9.59 9.75 10 9.75H14C14.41 9.75 14.75 10.09 14.75 10.5C14.75 10.91 14.41 11.25 14 11.25Z" fill="{color}"/>
<path d="M12 16.25C11.59 16.25 11.25 15.91 11.25 15.5V13.5C11.25 13.09 11.59 12.75 12 12.75C12.41 12.75 12.75 13.09 12.75 13.5V15.5C12.75 15.91 12.41 16.25 12 16.25Z" fill="{color}"/>
<path d="M14 14.25H10C9.59 14.25 9.25 13.91 9.25 13.5C9.25 13.09 9.59 12.75 10 12.75H14C14.41 12.75 14.75 13.09 14.75 13.5C14.75 13.91 14.41 14.25 14 14.25Z" fill="{color}"/>
<path d="M15 22.75H9C3.57 22.75 1.25 20.43 1.25 15V9C1.25 3.57 3.57 1.25 9 1.25H15C20.43 1.25 22.75 3.57 22.75 9V15C22.75 20.43 20.43 22.75 15 22.75ZM9 2.75C4.39 2.75 2.75 4.39 2.75 9V15C2.75 19.61 4.39 21.25 9 21.25H15C19.61 21.25 21.25 19.61 21.25 15V9C21.25 4.39 19.61 2.75 15 2.75H9Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<g opacity="0.4">
<path d="M15.15 18H8.84998C7.82998 18 7 17.17 7 16.15V7.85C7 6.83 7.82998 6 8.84998 6H15.15C16.17 6 17 6.83 17 7.85V16.15C17 17.17 16.17 18 15.15 18Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 8.5V10.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10 10.5H14" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 15.5V13.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10 13.5H14" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</g>
<path d="M15 22H9C4 22 2 20 2 15V9C2 4 4 2 9 2H15C20 2 22 4 22 9V15C22 20 20 22 15 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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