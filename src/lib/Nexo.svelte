<script lang="ts">
	export let color = 'currentColor';
	export let variant: 'linear' | 'bold' | 'broken' | 'bulk' | 'outline' | 'twotone' = 'linear';
	export let size = '1em';
	export let axis_y = '-0.12em';
	export let axis_x = '0';
	export let flip_x = false;
	export let flip_y = false;
	export let rotate = 0;	
</script>

<span style="width: {size}; height: {size}; bottom: {axis_y}; left: {axis_x}; transform: rotate({rotate}deg);" class:horizontal-reverted={flip_x} class:vertical-reverted={flip_y}>
	{#if variant == 'linear'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 6L17 3L22 6V18L17 21L7 15V9L17 15V9L12 6Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 6L7 3L2 6V18L7 21L11.7 17.87" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M22 6.27968V17.7097C22 17.8897 21.91 18.0497 21.76 18.1397L18.87 19.8697C18.71 19.9597 18.52 19.9597 18.36 19.8697L8.75 14.2797C8.6 14.1897 8.5 14.0297 8.5 13.8497V12.5197C8.5 12.1297 8.91999 11.8897 9.25999 12.0897L17.75 17.1797C18.08 17.3797 18.51 17.1397 18.51 16.7497V8.41968C18.51 8.23968 18.42 8.07969 18.27 7.98969L14.19 5.53968C13.87 5.34968 13.87 4.87968 14.19 4.67968L16.76 3.12969C16.92 3.02969 17.12 3.02969 17.28 3.12969L21.78 5.82968C21.91 5.93968 22 6.10968 22 6.27968Z" fill="{color}"/>
<path d="M11.2898 18.4309L7.25977 20.8509C7.09977 20.9509 6.89977 20.9509 6.74977 20.8509L2.24977 18.1509C2.09977 18.0609 2.00977 17.9009 2.00977 17.7209V6.29093C2.00977 6.11093 2.09977 5.95093 2.24977 5.86093L6.74977 3.16094C6.90977 3.06094 7.10977 3.06094 7.25977 3.16094L16.7598 8.86093C16.9098 8.95093 16.9998 9.11093 16.9998 9.29093V14.1209C16.9998 14.5109 16.5798 14.7509 16.2398 14.5509L7.74977 9.46094C7.41977 9.26094 6.98978 9.50093 6.98978 9.89093V14.7209C6.98978 14.9009 7.07977 15.0609 7.22977 15.1509L11.2698 17.5809C11.6098 17.7709 11.6098 18.2309 11.2898 18.4309Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 6L17 3L22 6V18L17 21L7 15V9L17 15V9L12 6Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 12V18L7 21L11.7 17.87" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 6L7 3L2 6V8.05" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" d="M16 8l6.667-4 6.667 4v16l-6.667 4-13.333-8v-8l13.333 8v-8l-6.667-4z"></path>
<path fill="{color}" opacity="0.4" d="M16 24l-6.667 4-6.667-4v-16l6.667-4 13.333 8v8l-13.333-8v8l6.667 4z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M17 21.7501C16.87 21.7501 16.73 21.7101 16.61 21.6401L6.61 15.6401C6.38 15.5001 6.25 15.2601 6.25 15.0001V9.00014C6.25 8.73014 6.4 8.48015 6.63 8.35015C6.87 8.22015 7.15 8.22014 7.39 8.36014L16.25 13.6801V9.43013L11.61 6.65014C11.38 6.51014 11.25 6.27014 11.25 6.01014C11.25 5.75014 11.39 5.50014 11.61 5.37014L16.61 2.37014C16.85 2.23014 17.14 2.23014 17.38 2.37014L22.38 5.37014C22.61 5.51014 22.74 5.75014 22.74 6.01014V18.0101C22.74 18.2701 22.6 18.5201 22.38 18.6501L17.38 21.6501C17.27 21.7101 17.13 21.7501 17 21.7501ZM7.75 14.5801L17 20.1301L21.25 17.5801V6.43013L17 3.88015L13.46 6.01014L17.39 8.37014C17.62 8.51014 17.75 8.75014 17.75 9.01014V15.0101C17.75 15.2801 17.6 15.5301 17.37 15.6601C17.14 15.7901 16.85 15.7901 16.61 15.6501L7.75 10.3301V14.5801Z" fill="{color}"/>
<path d="M7 21.7499C6.87 21.7499 6.73 21.7099 6.61 21.6399L1.61 18.6399C1.38 18.4999 1.25 18.2599 1.25 17.9999V5.99988C1.25 5.73988 1.39 5.48988 1.61 5.35988L6.61 2.35988C6.85 2.21988 7.14001 2.21988 7.38 2.35988L12.38 5.35988C12.74 5.56988 12.85 6.02988 12.64 6.38988C12.43 6.74988 11.97 6.85988 11.61 6.64988L7 3.87989L2.75 6.42987V17.5799L6.98 20.1199L11.29 17.2499C11.63 17.0199 12.1 17.1099 12.33 17.4599C12.56 17.8099 12.47 18.2699 12.12 18.4999L7.42 21.6299C7.29 21.7099 7.15 21.7499 7 21.7499Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 6L17 3L22 6V18L17 21L7 15V9L17 15V9L12 6Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M12 6L7 3L2 6V18L7 21L11.7 17.87" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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