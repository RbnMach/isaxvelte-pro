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
<path d="M16.0001 5H19.5001L22.2001 9.7L17.0001 19L15.1001 15.9L18.7001 9.7L16.0001 5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9.0001 5H12.5001L15.2001 9.7L10.0001 19L8.1001 15.9L11.7001 9.7L9.0001 5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M1.80005 5H5.30005L8.00005 9.8L6.30005 12.7L1.80005 5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.8604 5H19.2104C19.3904 5 19.5504 5.1 19.6404 5.25L22.0504 9.45C22.1404 9.6 22.1404 9.79 22.0504 9.94L17.4104 18.24C17.2204 18.58 16.7404 18.58 16.5404 18.25L15.2804 16.14C15.1904 15.98 15.1904 15.79 15.2804 15.64L18.5404 9.94C18.6304 9.79 18.6304 9.6 18.5404 9.44L16.4104 5.74001C16.2404 5.42001 16.4804 5 16.8604 5Z" fill="{color}"/>
<path d="M9.86038 5H12.2104C12.3904 5 12.5504 5.1 12.6404 5.25L15.0504 9.45C15.1404 9.6 15.1404 9.79 15.0504 9.94L10.4104 18.24C10.2204 18.58 9.7404 18.58 9.5404 18.25L8.28039 16.14C8.19039 15.98 8.19039 15.79 8.28039 15.64L11.5404 9.94C11.6304 9.79 11.6304 9.6 11.5404 9.44L9.4104 5.74001C9.2404 5.42001 9.48038 5 9.86038 5Z" fill="{color}"/>
<path d="M1.80078 5H5.0108C5.1908 5 5.36081 5.1 5.45081 5.25L7.87079 9.53999C7.96079 9.68999 7.96079 9.87999 7.87079 10.04L6.75079 11.96C6.56079 12.29 6.08081 12.29 5.89081 11.96L1.80078 5Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.0004 5H19.5004L22.2004 9.7L17.0004 19L15.1504 15.9L18.7004 9.7L16.0004 5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10.8404 17.49L10.0004 19L8.15039 15.9L11.7004 9.7L9.0004 5H12.5004L15.2004 9.7L12.9304 13.77" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M1.80078 5H5.30078L8.00079 9.8L6.30078 12.7L1.80078 5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" d="M22.481 6.667h3.133c0.24 0 0.453 0.133 0.573 0.333l3.213 5.6c0.12 0.2 0.12 0.453 0 0.653l-6.187 11.067c-0.253 0.453-0.893 0.453-1.16 0.013l-1.68-2.813c-0.12-0.213-0.12-0.467 0-0.667l4.347-7.6c0.12-0.2 0.12-0.453 0-0.667l-2.84-4.933c-0.227-0.427 0.093-0.987 0.6-0.987z"></path>
<path fill="{color}" opacity="0.4" d="M13.147 6.667h3.133c0.24 0 0.453 0.133 0.573 0.333l3.213 5.6c0.12 0.2 0.12 0.453 0 0.653l-6.187 11.067c-0.253 0.453-0.893 0.453-1.16 0.013l-1.68-2.813c-0.12-0.213-0.12-0.467 0-0.667l4.347-7.6c0.12-0.2 0.12-0.453 0-0.667l-2.84-4.933c-0.227-0.427 0.093-0.987 0.6-0.987z"></path>
<path fill="{color}" d="M2.401 6.667h4.28c0.24 0 0.467 0.133 0.587 0.333l3.227 5.72c0.12 0.2 0.12 0.453 0 0.667l-1.493 2.56c-0.253 0.44-0.893 0.44-1.147 0l-5.453-9.28z"></path>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.9996 19.7502C16.7396 19.7502 16.4896 19.6102 16.3596 19.3802L14.5096 16.2802C14.3696 16.0502 14.3696 15.7602 14.4996 15.5202L17.8396 9.69023L15.3496 5.36023C15.2196 5.13023 15.2196 4.84023 15.3496 4.61023C15.4796 4.38023 15.7296 4.24023 15.9996 4.24023H19.4996C19.7696 4.24023 20.0196 4.38022 20.1496 4.62022L22.8496 9.32024C22.9796 9.55024 22.9796 9.83023 22.8496 10.0602L17.6496 19.3602C17.5196 19.5902 17.2696 19.7402 17.0096 19.7402C17.0096 19.7502 16.9996 19.7502 16.9996 19.7502ZM16.0196 15.8902L16.9796 17.5002L21.3396 9.70023L19.0696 5.74023H17.2996L19.3496 9.32024C19.4796 9.55024 19.4796 9.84024 19.3496 10.0702L16.0196 15.8902Z" fill="{color}"/>
<path d="M9.9996 19.7502C9.7396 19.7502 9.48959 19.6102 9.35959 19.3802L7.50961 16.2802C7.36961 16.0502 7.3696 15.7602 7.4996 15.5202L10.8396 9.69023L8.34961 5.36023C8.21961 5.13023 8.21961 4.84023 8.34961 4.61023C8.47961 4.38023 8.7296 4.24023 8.9996 4.24023H12.4996C12.7696 4.24023 13.0196 4.38022 13.1496 4.62022L15.8496 9.32024C15.9796 9.55024 15.9796 9.83023 15.8496 10.0602L10.6496 19.3602C10.5196 19.5902 10.2696 19.7402 10.0096 19.7402C10.0096 19.7502 9.9996 19.7502 9.9996 19.7502ZM9.01959 15.8902L9.97961 17.5002L14.3396 9.70023L12.0696 5.74023H10.2996L12.3496 9.32024C12.4796 9.55024 12.4796 9.84024 12.3496 10.0702L9.01959 15.8902Z" fill="{color}"/>
<path d="M6.29992 13.45C6.02992 13.45 5.78992 13.31 5.64992 13.08L1.14992 5.38C1.00992 5.15 1.00992 4.86 1.14992 4.63C1.27992 4.4 1.52992 4.25 1.79992 4.25H5.29992C5.56992 4.25 5.81994 4.4 5.94994 4.63L8.64992 9.42999C8.77992 9.65999 8.77994 9.94999 8.63994 10.18L6.93993 13.08C6.80993 13.31 6.56992 13.45 6.29992 13.45ZM3.10991 5.75L6.29992 11.22L7.12993 9.8L4.85991 5.75999H3.10991V5.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.0004 5H19.5004L22.2004 9.7L17.0004 19L15.1504 15.9L18.7004 9.7L16.0004 5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M9.0004 5H12.5004L15.2004 9.7L10.0004 19L8.15039 15.9L11.7004 9.7L9.0004 5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M1.7998 5H5.2998L7.99982 9.8L6.2998 12.7L1.7998 5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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