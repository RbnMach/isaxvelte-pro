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
<path d="M7.46995 3.3501H16.53C17.59 3.3501 18.84 4.1201 19.31 5.0701L21.71 9.8901C22.29 11.0501 21.97 12.7001 21.02 13.5701L14.09 19.8601C12.94 20.9001 11.07 20.9001 9.91996 19.8601L2.98996 13.5701C2.02996 12.7001 1.71996 11.0501 2.29996 9.8901L4.69996 5.0701C5.15996 4.1201 6.40996 3.3501 7.46995 3.3501Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 14.5V8.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8 8.5H16" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M21.7101 9.89937L19.3101 5.07938C18.8401 4.12938 17.5901 3.35938 16.5301 3.35938H7.4701C6.4101 3.35938 5.1601 4.12938 4.6901 5.07938L2.29009 9.89937C1.71009 11.0594 2.03009 12.7094 2.98009 13.5794L9.9101 19.8694C11.0601 20.9094 12.9301 20.9094 14.0801 19.8694L21.0101 13.5794C21.9701 12.7094 22.2901 11.0494 21.7101 9.89937ZM16.0001 9.24938H12.7501V14.4994C12.7501 14.9094 12.4101 15.2494 12.0001 15.2494C11.5901 15.2494 11.2501 14.9094 11.2501 14.4994V9.24938H8.0001C7.5901 9.24938 7.2501 8.90938 7.2501 8.49938C7.2501 8.08938 7.5901 7.74938 8.0001 7.74938H16.0001C16.4101 7.74938 16.7501 8.08938 16.7501 8.49938C16.7501 8.90938 16.4101 9.24938 16.0001 9.24938Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M18.1004 16.2201L14.0804 19.8701C12.9304 20.9101 11.0604 20.9101 9.91044 19.8701L2.98044 13.5801C2.02044 12.7101 1.71043 11.0601 2.29043 9.90011L4.69044 5.08011C5.16044 4.13011 6.41044 3.36011 7.47044 3.36011H16.5304C17.5904 3.36011 18.8404 4.13011 19.3104 5.08011L21.7104 9.90011C22.2904 11.0601 21.9704 12.7101 21.0204 13.5801" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 14.5V8.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8 8.5H16" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M9.96 4.467h12.080c1.413 0 3.080 1.027 3.707 2.293l3.2 6.427c0.773 1.547 0.347 3.747-0.92 4.907l-9.24 8.387c-1.533 1.387-4.027 1.387-5.56 0l-9.24-8.387c-1.28-1.16-1.693-3.36-0.92-4.907l3.2-6.427c0.613-1.267 2.28-2.293 3.693-2.293z"></path>
<path fill="{color}" d="M21.333 10.333h-10.667c-0.547 0-1 0.453-1 1s0.453 1 1 1h4.333v7c0 0.547 0.453 1 1 1s1-0.453 1-1v-7h4.333c0.547 0 1-0.453 1-1s-0.453-1-1-1z"></path>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11.9997 21.3999C11.0597 21.3999 10.1197 21.0799 9.40973 20.4299L2.47972 14.1399C1.26972 13.0399 0.889723 11.0299 1.61972 9.56986L4.01973 4.74986C4.61973 3.54986 6.12973 2.60986 7.46973 2.60986H16.5297C17.8697 2.60986 19.3797 3.54986 19.9797 4.74986L22.3797 9.56986C23.1097 11.0299 22.7297 13.0399 21.5197 14.1399L14.5897 20.4299C13.8797 21.0699 12.9397 21.3999 11.9997 21.3999ZM7.46973 4.09986C6.68973 4.09986 5.70973 4.70986 5.35973 5.40986L2.95973 10.2299C2.53973 11.0799 2.77973 12.3799 3.48973 13.0199L10.4197 19.3099C11.2797 20.0899 12.7297 20.0899 13.5797 19.3099L20.5097 13.0199C21.2097 12.3799 21.4597 11.0799 21.0397 10.2299L18.6397 5.40986C18.2897 4.71986 17.3097 4.10986 16.5297 4.10986H7.46973V4.09986Z" fill="{color}"/>
<path d="M12 15.25C11.59 15.25 11.25 14.91 11.25 14.5V8.5C11.25 8.09 11.59 7.75 12 7.75C12.41 7.75 12.75 8.09 12.75 8.5V14.5C12.75 14.91 12.41 15.25 12 15.25Z" fill="{color}"/>
<path d="M16 9.25H8C7.59 9.25 7.25 8.91 7.25 8.5C7.25 8.09 7.59 7.75 8 7.75H16C16.41 7.75 16.75 8.09 16.75 8.5C16.75 8.91 16.41 9.25 16 9.25Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M7.4702 3.3501H16.5302C17.5902 3.3501 18.8402 4.1201 19.3102 5.0701L21.7102 9.8901C22.2902 11.0501 21.9702 12.7001 21.0202 13.5701L14.0902 19.8601C12.9402 20.9001 11.0702 20.9001 9.92019 19.8601L2.9902 13.5701C2.0302 12.7001 1.7202 11.0501 2.3002 9.8901L4.70019 5.0701C5.16019 4.1201 6.4102 3.3501 7.4702 3.3501Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<g opacity="0.4">
<path d="M12 14.5V8.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8 8.5H16" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</g>
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