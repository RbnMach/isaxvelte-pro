<script lang="ts">
	export let color = 'currentColor';
	export let variant: 'linear' | 'bold' | 'broken' | 'bulk' | 'outline' | 'twotone' = 'linear';
	export let size = '1.1em';
	export let axis_y = '-0.13em';
	export let axis_x = '0';
	export let flip_x = false;
	export let flip_y = false;
	export let rotate = 0;	
</script>

<span style="width: {size}; height: {size}; bottom: {axis_y}; left: {axis_x}; transform: rotate({rotate}deg);" class:horizontal-reverted={flip_x} class:vertical-reverted={flip_y}>
	{#if variant == 'linear'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M9.51002 4.23001L18.07 8.51001C21.91 10.43 21.91 13.57 18.07 15.49L9.51002 19.77C3.75002 22.65 1.40002 20.29 4.28002 14.54L5.15002 12.81C5.37002 12.37 5.37002 11.64 5.15002 11.2L4.28002 9.46001C1.40002 3.71001 3.76002 1.35001 9.51002 4.23001Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5.44 12H10.84" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M18.0693 8.50867L9.50929 4.22867C3.75929 1.34867 1.39929 3.70867 4.27929 9.45867L5.14929 11.1987C5.39929 11.7087 5.39929 12.2987 5.14929 12.8087L4.27929 14.5387C1.39929 20.2887 3.74929 22.6487 9.50929 19.7687L18.0693 15.4887C21.9093 13.5687 21.9093 10.4287 18.0693 8.50867ZM14.8393 12.7487H9.43929C9.02929 12.7487 8.68929 12.4087 8.68929 11.9987C8.68929 11.5887 9.02929 11.2487 9.43929 11.2487H14.8393C15.2493 11.2487 15.5893 11.5887 15.5893 11.9987C15.5893 12.4087 15.2493 12.7487 14.8393 12.7487Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M18.0693 8.50989C21.9093 10.4299 21.9093 13.5699 18.0693 15.4899L9.50929 19.7699C3.74929 22.6499 1.39929 20.2899 4.27929 14.5399L5.14929 12.8099C5.36929 12.3699 5.36929 11.6399 5.14929 11.1999L4.27929 9.45989C1.39929 3.70989 3.75929 1.34989 9.50929 4.22989L14.0193 6.48989" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5.43945 12H10.8395" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M9.50929 4.22989L18.0693 8.50989C21.9093 10.4299 21.9093 13.5699 18.0693 15.4899L9.50929 19.7699C3.74929 22.6499 1.39929 20.2899 4.27929 14.5399L5.14929 12.8099C5.39929 12.2999 5.39929 11.7099 5.14929 11.1999L4.27929 9.45989C1.39929 3.70989 3.75929 1.34989 9.50929 4.22989Z" fill="{color}"/>
<path d="M14.8395 12.75H9.43945C9.02945 12.75 8.68945 12.41 8.68945 12C8.68945 11.59 9.02945 11.25 9.43945 11.25H14.8395C15.2495 11.25 15.5895 11.59 15.5895 12C15.5895 12.41 15.2495 12.75 14.8395 12.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5.40995 21.7499C4.28995 21.7499 3.57995 21.3699 3.12995 20.9199C2.24995 20.0399 1.62995 18.1699 3.60995 14.1999L4.47995 12.4699C4.58995 12.2399 4.58995 11.7599 4.47995 11.5299L3.60995 9.7999C1.61995 5.8299 2.24995 3.9499 3.12995 3.0799C3.99995 2.1999 5.87995 1.5699 9.83995 3.5599L18.3999 7.8399C20.5299 8.8999 21.6999 10.3799 21.6999 11.9999C21.6999 13.6199 20.5299 15.0999 18.4099 16.1599L9.84995 20.4399C7.90995 21.4099 6.46995 21.7499 5.40995 21.7499ZM5.40995 3.7499C4.86995 3.7499 4.44995 3.8799 4.18995 4.1399C3.45995 4.8599 3.74995 6.7299 4.94995 9.1199L5.81995 10.8599C6.13995 11.5099 6.13995 12.4899 5.81995 13.1399L4.94995 14.8699C3.74995 17.2699 3.45995 19.1299 4.18995 19.8499C4.90995 20.5799 6.77995 20.2899 9.17995 19.0899L17.7399 14.8099C19.3099 14.0299 20.1999 12.9999 20.1999 11.9899C20.1999 10.9799 19.2999 9.9499 17.7299 9.1699L9.16995 4.8999C7.64995 4.1399 6.33995 3.7499 5.40995 3.7499Z" fill="{color}"/>
<path d="M10.8395 12.75H5.43945C5.02945 12.75 4.68945 12.41 4.68945 12C4.68945 11.59 5.02945 11.25 5.43945 11.25H10.8395C11.2495 11.25 11.5895 11.59 11.5895 12C11.5895 12.41 11.2495 12.75 10.8395 12.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M9.50929 4.23013L18.0693 8.51013C21.9093 10.4301 21.9093 13.5701 18.0693 15.4901L9.50929 19.7701C3.74929 22.6501 1.39929 20.2901 4.27929 14.5401L5.14929 12.8101C5.36929 12.3701 5.36929 11.6401 5.14929 11.2001L4.27929 9.46013C1.39929 3.71013 3.75929 1.35013 9.50929 4.23013Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.34" d="M5.43945 12H10.8395" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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