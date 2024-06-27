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
<path d="M9.5 3.19995H14.5C18.3 3.19995 21.5 6.29995 21.5 10.2C21.5 14 18.4 17.2 14.5 17.2H3.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3.2002 6.80005H13.8002C15.8002 6.80005 17.5002 8.50005 17.5002 10.5C17.5002 12.5 15.8002 14.2 13.8002 14.2H8.0002" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.5 10.8H5.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6.5 20.8H2.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M14.5 18H3.5C3.09 18 2.75 17.66 2.75 17.25C2.75 16.84 3.09 16.5 3.5 16.5H14.5C17.95 16.5 20.75 13.7 20.75 10.25C20.75 6.8 17.95 4 14.5 4H9.5C9.09 4 8.75 3.66 8.75 3.25C8.75 2.84 9.09 2.5 9.5 2.5H14.5C18.77 2.5 22.25 5.98 22.25 10.25C22.25 14.52 18.77 18 14.5 18Z" fill="{color}"/>
<path d="M13.8099 14.8917H7.99994C7.58994 14.8917 7.24994 14.5517 7.24994 14.1417C7.24994 13.7317 7.58994 13.3917 7.99994 13.3917H13.8099C15.4299 13.3917 16.7499 12.0717 16.7499 10.4517C16.7499 8.83172 15.4299 7.51172 13.8099 7.51172H3.16992C2.75992 7.51172 2.41992 7.17172 2.41992 6.76172C2.41992 6.35172 2.75992 6.01172 3.16992 6.01172H13.8099C16.2599 6.01172 18.2499 8.00172 18.2499 10.4517C18.2499 12.9017 16.2599 14.8917 13.8099 14.8917Z" fill="{color}"/>
<path d="M8.5 11.5H5.5C5.09 11.5 4.75 11.16 4.75 10.75C4.75 10.34 5.09 10 5.5 10H8.5C8.91 10 9.25 10.34 9.25 10.75C9.25 11.16 8.91 11.5 8.5 11.5Z" fill="{color}"/>
<path d="M6.5 21.5H2.5C2.09 21.5 1.75 21.16 1.75 20.75C1.75 20.34 2.09 20 2.5 20H6.5C6.91 20 7.25 20.34 7.25 20.75C7.25 21.16 6.91 21.5 6.5 21.5Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M19.72 14.8999C18.44 16.3399 16.57 17.2499 14.5 17.2499H3.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9.5 3.25H14.5C18.35 3.25 21.5 6.4 21.5 10.25" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3.16992 6.75H13.8099C15.8399 6.75 17.4999 8.41 17.4999 10.44C17.4999 12.47 15.8399 14.13 13.8099 14.13H7.99994" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.5 10.75H5.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6.5 20.75H2.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" d="M19.333 24h-14.667c-0.547 0-1-0.453-1-1s0.453-1 1-1h14.667c4.6 0 8.333-3.733 8.333-8.333s-3.733-8.333-8.333-8.333h-6.667c-0.547 0-1-0.453-1-1s0.453-1 1-1h6.667c5.693 0 10.333 4.64 10.333 10.333s-4.64 10.333-10.333 10.333z"></path>
<path fill="{color}" opacity="0.4" d="M18.413 19.853h-7.747c-0.547 0-1-0.453-1-1s0.453-1 1-1h7.747c2.16 0 3.92-1.76 3.92-3.92s-1.76-3.92-3.92-3.92h-14.187c-0.547 0-1-0.453-1-1s0.44-1.013 1-1.013h14.187c3.267 0 5.92 2.653 5.92 5.92s-2.653 5.933-5.92 5.933z"></path>
<path fill="{color}" d="M11.333 15.333h-4c-0.547 0-1-0.453-1-1s0.453-1 1-1h4c0.547 0 1 0.453 1 1s-0.453 1-1 1z"></path>
<path fill="{color}" opacity="0.4" d="M8.667 28.667h-5.333c-0.547 0-1-0.453-1-1s0.453-1 1-1h5.333c0.547 0 1 0.453 1 1s-0.453 1-1 1z"></path>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M14.5 18H3.5C3.09 18 2.75 17.66 2.75 17.25C2.75 16.84 3.09 16.5 3.5 16.5H14.5C17.95 16.5 20.75 13.7 20.75 10.25C20.75 6.8 17.95 4 14.5 4H9.5C9.09 4 8.75 3.66 8.75 3.25C8.75 2.84 9.09 2.5 9.5 2.5H14.5C18.77 2.5 22.25 5.98 22.25 10.25C22.25 14.52 18.77 18 14.5 18Z" fill="{color}"/>
<path d="M13.8099 14.8898H7.99994C7.58994 14.8898 7.24994 14.5498 7.24994 14.1398C7.24994 13.7298 7.58994 13.3898 7.99994 13.3898H13.8099C15.4299 13.3898 16.7499 12.0698 16.7499 10.4498C16.7499 8.82977 15.4299 7.50977 13.8099 7.50977H3.16992C2.75992 7.50977 2.41992 7.16977 2.41992 6.75977C2.41992 6.34977 2.75992 6.00977 3.16992 6.00977H13.8099C16.2599 6.00977 18.2499 7.99977 18.2499 10.4498C18.2499 12.8998 16.2599 14.8898 13.8099 14.8898Z" fill="{color}"/>
<path d="M8.5 11.5H5.5C5.09 11.5 4.75 11.16 4.75 10.75C4.75 10.34 5.09 10 5.5 10H8.5C8.91 10 9.25 10.34 9.25 10.75C9.25 11.16 8.91 11.5 8.5 11.5Z" fill="{color}"/>
<path d="M6.5 21.5H2.5C2.09 21.5 1.75 21.16 1.75 20.75C1.75 20.34 2.09 20 2.5 20H6.5C6.91 20 7.25 20.34 7.25 20.75C7.25 21.16 6.91 21.5 6.5 21.5Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M9.5 3.25H14.5C18.35 3.25 21.5 6.4 21.5 10.25C21.5 14.1 18.35 17.25 14.5 17.25H3.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M3.16992 6.75H13.8099C15.8399 6.75 17.4999 8.41 17.4999 10.44C17.4999 12.47 15.8399 14.13 13.8099 14.13H7.99994" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M8.5 10.75H5.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M6.5 20.75H2.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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