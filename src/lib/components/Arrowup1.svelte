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
<path d="M19.9201 15.0499L13.4001 8.52989C12.6301 7.75989 11.3701 7.75989 10.6001 8.52989L4.08008 15.0499" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M18.6806 13.9783L15.4706 10.7683L13.5106 8.79828C12.6806 7.96828 11.3306 7.96828 10.5006 8.79828L5.32056 13.9783C4.64056 14.6583 5.13056 15.8183 6.08056 15.8183H11.6906H17.9206C18.8806 15.8183 19.3606 14.6583 18.6806 13.9783Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.0101 11.1499L13.4001 8.52989C12.6301 7.75989 11.3701 7.75989 10.6001 8.52989L4.08008 15.0499" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M19.9209 15.05L18.8809 14.01" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M15.4807 10.7702L11.6907 15.8202H6.08072C5.12072 15.8202 4.64073 14.6602 5.32073 13.9802L10.5007 8.80023C11.3307 7.97023 12.6807 7.97023 13.5107 8.80023L15.4807 10.7702Z" fill="{color}"/>
<path d="M17.9195 15.82H11.6895L15.4795 10.77L18.6895 13.98C19.3595 14.66 18.8795 15.82 17.9195 15.82Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M19.9195 15.8001C19.7295 15.8001 19.5395 15.7301 19.3895 15.5801L12.8695 9.06008C12.3895 8.58008 11.6095 8.58008 11.1295 9.06008L4.60953 15.5801C4.31953 15.8701 3.83953 15.8701 3.54953 15.5801C3.25953 15.2901 3.25953 14.8101 3.54953 14.5201L10.0695 8.00008C11.1295 6.94008 12.8595 6.94008 13.9295 8.00008L20.4495 14.5201C20.7395 14.8101 20.7395 15.2901 20.4495 15.5801C20.2995 15.7201 20.1095 15.8001 19.9195 15.8001Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M19.9201 15.0501L13.4001 8.53014C12.6301 7.76014 11.3701 7.76014 10.6001 8.53014L4.08008 15.0501" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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