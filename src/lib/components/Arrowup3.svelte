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
<path d="M18.0701 9.57L12.0001 3.5L5.93005 9.57" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 20.4999V3.66992" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.19 2H7.81C4.17 2 2 4.17 2 7.81V16.18C2 19.83 4.17 22 7.81 22H16.18C19.82 22 21.99 19.83 21.99 16.19V7.81C22 4.17 19.83 2 16.19 2ZM16.82 10.82C16.53 11.11 16.05 11.11 15.76 10.82L12.75 7.81V18C12.75 18.41 12.41 18.75 12 18.75C11.59 18.75 11.25 18.41 11.25 18V7.81L8.24 10.82C7.95 11.11 7.47 11.11 7.18 10.82C7.03 10.67 6.96 10.48 6.96 10.29C6.96 10.1 7.04 9.9 7.18 9.76L11.47 5.47C11.61 5.33 11.8 5.25 12 5.25C12.2 5.25 12.39 5.33 12.53 5.47L16.82 9.76C17.11 10.05 17.11 10.52 16.82 10.82Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M18.0697 9.57L11.9997 3.5L5.92969 9.57" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 11.9999V3.66992" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 20.5V15.97" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M22 7.81V16.18C22 19.82 19.83 21.99 16.19 21.99H7.81C4.17 22 2 19.83 2 16.19V7.81C2 4.17 4.17 2 7.81 2H16.18C19.83 2 22 4.17 22 7.81Z" fill="{color}"/>
<path d="M12.5309 5.47L16.8209 9.76C17.1109 10.05 17.1109 10.53 16.8209 10.82C16.5309 11.11 16.0509 11.11 15.7609 10.82L12.7509 7.81V18C12.7509 18.41 12.4109 18.75 12.0009 18.75C11.5909 18.75 11.2509 18.41 11.2509 18V7.81L8.24094 10.82C7.95094 11.11 7.47094 11.11 7.18094 10.82C7.03094 10.67 6.96094 10.48 6.96094 10.29C6.96094 10.1 7.04094 9.9 7.18094 9.76L11.4709 5.47C11.6109 5.33 11.8009 5.25 12.0009 5.25C12.2009 5.25 12.3909 5.33 12.5309 5.47Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M18.0691 10.3199C17.8791 10.3199 17.6891 10.2499 17.5391 10.0999L11.9991 4.55994L6.45914 10.0999C6.16914 10.3899 5.68914 10.3899 5.39914 10.0999C5.10914 9.80994 5.10914 9.32994 5.39914 9.03994L11.4691 2.96994C11.7591 2.67994 12.2391 2.67994 12.5291 2.96994L18.5991 9.03994C18.8891 9.32994 18.8891 9.80994 18.5991 10.0999C18.4591 10.2499 18.2591 10.3199 18.0691 10.3199Z" fill="{color}"/>
<path d="M12 21.2499C11.59 21.2499 11.25 20.9099 11.25 20.4999V3.66992C11.25 3.25992 11.59 2.91992 12 2.91992C12.41 2.91992 12.75 3.25992 12.75 3.66992V20.4999C12.75 20.9099 12.41 21.2499 12 21.2499Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M18.0697 9.57L11.9997 3.5L5.92969 9.57" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M12 20.4999V3.66992" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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