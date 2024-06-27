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
<path d="M12 5.19995L9.5 13.2L14.5 10.8L12 5.19995Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M14.1 11L18 12.2L13.5 14.8L13.1 14.6L6 12.2L10 10.2" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M13 15.1999L12 18.1999L9.5 13.5999" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM13.5 14.75L13.19 14.65L13 15.25L12 18.25L9.5 13.57L9.39999 13.38L6 12.25L8.17999 11.16L10 10.25L10.47 10.04L12 5.25L13.55 8.64999L14.5 10.75L14.09 10.96L18 12.25L13.5 14.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 5.25L9.5 13.25L14.5 10.75L12 5.25Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M14.08 10.96L18 12.25L13.5 14.75L13.1 14.62L6 12.25L10 10.25" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M13 15.2501L12 18.2501L9.5 13.5701" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.2 2.30001 7.97 2.85001" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M19.334 14.333l-0.547 0.28h-0.013l-6.24 3.227 1.427-4.453 4.107-1.853 1.267 2.8z"></path>
<path fill="{color}" d="M18.068 11.533l-4.107 1.853 2.040-6.387 2.067 4.533z"></path>
<path fill="{color}" d="M13.96 13.387l-1.427 4.453-4.533-1.507 5.333-2.667 0.627-0.28z"></path>
<path fill="{color}" d="M24.001 16.333l-6 3.333-0.413-0.133-0.12-0.040-4.933-1.653 6.24-3.227h0.013l5.213 1.72z"></path>
<path fill="{color}" d="M17.587 19.533l-0.253 0.8-1.333 4-3.333-6.24-0.133-0.253 5.053 1.693z"></path>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M9.5005 13.9998C9.3305 13.9998 9.15051 13.9398 9.01051 13.8198C8.78051 13.6198 8.69049 13.3098 8.78049 13.0298L11.2805 5.02982C11.3705 4.72982 11.6405 4.51981 11.9505 4.50981C12.2705 4.48981 12.5505 4.66982 12.6805 4.94982L15.1805 10.4498C15.3505 10.8198 15.1905 11.2498 14.8305 11.4298L9.83048 13.9298C9.73048 13.9698 9.6105 13.9998 9.5005 13.9998ZM12.1305 7.34983L10.7405 11.7898L13.5205 10.3998L12.1305 7.34983Z" fill="{color}"/>
<path d="M13.4997 15.4999C13.4197 15.4999 13.3397 15.4899 13.2597 15.4599L5.75974 12.9599C5.46974 12.8599 5.26973 12.5999 5.24973 12.2999C5.22973 11.9999 5.38973 11.7099 5.65973 11.5799L9.65973 9.57994C10.0297 9.39994 10.4797 9.54994 10.6697 9.91994C10.8597 10.2899 10.7097 10.7399 10.3297 10.9299L7.94974 12.1199L13.4197 13.9399L16.1397 12.4299L13.8497 11.6699C13.4597 11.5399 13.2397 11.1199 13.3697 10.7199C13.4997 10.3299 13.9197 10.1099 14.3197 10.2399L18.2397 11.5299C18.5197 11.6199 18.7197 11.8799 18.7497 12.1699C18.7797 12.4699 18.6297 12.7499 18.3697 12.8999L13.8697 15.3999C13.7497 15.4699 13.6297 15.4999 13.4997 15.4999Z" fill="{color}"/>
<path d="M12.0003 18.9999C11.7203 18.9999 11.4703 18.8499 11.3403 18.5999L8.84028 13.9199C8.64028 13.5499 8.78028 13.0998 9.15028 12.8998C9.52028 12.6998 9.9703 12.8399 10.1703 13.2099L11.8503 16.3499L12.3003 14.9999C12.4303 14.6099 12.8603 14.3999 13.2503 14.5299C13.6403 14.6599 13.8503 15.0898 13.7203 15.4798L12.7203 18.4798C12.6303 18.7598 12.3703 18.9599 12.0703 18.9899C12.0403 18.9999 12.0203 18.9999 12.0003 18.9999Z" fill="{color}"/>
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<g opacity="0.4">
<path d="M12 5.25L9.5 13.25L14.5 10.75L12 5.25Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M14.08 10.96L18 12.25L13.5 14.75L13.1 14.62L6 12.25L10 10.25" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M13 15.2498L12 18.2498L9.5 13.5698" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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
</style>