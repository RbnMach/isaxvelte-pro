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
<path d="M12 5L7.6 2L2 6L6.4 9L12 5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 5L16.4 2L22 6L17.6 9L12 5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 14L7.6 17L2 13L6.4 10L12 14Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 14L16.4 17L22 13L17.6 10L12 14Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M19 15.5V18.8L12.4 21.8C12.1 21.9 11.8 21.9 11.6 21.8L5 18.8V15.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11.9994 6.00127L6.43936 10.0013L3.18936 7.80126C2.60936 7.41126 2.59938 6.57128 3.16938 6.16128L6.99936 3.40127C7.33936 3.16127 7.79938 3.15128 8.13938 3.38128L11.9994 6.00127Z" fill="{color}"/>
<path d="M20.81 7.79881L17.56 9.99882L12 5.99882L15.86 3.38883C16.21 3.15883 16.66 3.15882 17 3.40882L20.83 6.16883C21.4 6.56883 21.39 7.40881 20.81 7.79881Z" fill="{color}"/>
<path d="M11.9999 14L7.55992 17L4.99992 15.16L3.15992 13.84C2.59992 13.43 2.60991 12.59 3.17991 12.2L6.42991 10L11.9999 14Z" fill="{color}"/>
<path d="M20.8102 12.2C21.3902 12.59 21.4002 13.43 20.8302 13.84L18.9902 15.16L16.4302 17L11.9902 14L17.5502 10L20.8102 12.2Z" fill="{color}"/>
<path d="M18.68 17.3381C18.81 17.2381 19 17.3381 19 17.4981V18.2281C19 18.6181 18.77 18.9681 18.42 19.1381L12.42 21.9081C12.15 22.0281 11.85 22.0281 11.58 21.9081L5.57999 19.1381C5.22999 18.9681 5 18.6181 5 18.2281V17.4981C5 17.3381 5.18001 17.2381 5.32001 17.3381L7.25 18.7281C7.42 18.8481 7.65001 18.8581 7.82001 18.7381L11.72 16.0981C11.89 15.9881 12.11 15.9881 12.28 16.0981L16.18 18.7381C16.35 18.8581 16.58 18.8481 16.75 18.7281L18.68 17.3381Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 5L7.56 2L2 6L6.44 9L12 5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 5L16.44 2L22 6L17.56 9L12 5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 14L7.56 17L2 13L6.44 10L8.51999 11.5L10.14 12.66L12 14Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 14L16.44 17L22 13L17.56 10L12 14Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5 18.77V15.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M18.9997 15.5V18.77L12.4197 21.81C12.1497 21.93 11.8497 21.93 11.5797 21.81L9.67969 20.93" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M15.999 8l-7.413 5.333-4.333-2.933c-0.773-0.52-0.787-1.64-0.027-2.187l5.107-3.68c0.453-0.32 1.067-0.333 1.52-0.027l5.147 3.493z"></path>
<path fill="{color}" opacity="0.4" d="M27.747 10.4l-4.333 2.933-7.413-5.333 5.147-3.48c0.467-0.307 1.067-0.307 1.52 0.027l5.107 3.68c0.76 0.533 0.747 1.653-0.027 2.173z"></path>
<path fill="{color}" opacity="0.4" d="M16 18.667l-5.92 4-5.867-4.213c-0.747-0.547-0.733-1.667 0.027-2.187l4.333-2.933 7.427 5.333z"></path>
<path fill="{color}" opacity="0.4" d="M27.747 16.267c0.773 0.52 0.787 1.64 0.027 2.187l-2.44 1.76-3.413 2.453-5.92-4 7.413-5.333 4.333 2.933z"></path>
<path fill="{color}" d="M25.333 20.213v3.96c0 0.52-0.307 0.987-0.773 1.213l-8 3.693c-0.36 0.16-0.76 0.16-1.12 0l-8-3.693c-0.467-0.213-0.773-0.693-0.773-1.213v-3.96l3.413 2.453 5.92-4 5.92 4 3.413-2.453z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M6.44 9.75009C6.29 9.75009 6.14999 9.71009 6.01999 9.62009L1.57999 6.62009C1.37999 6.48009 1.25 6.2501 1.25 6.0101C1.25 5.7601 1.36 5.53011 1.56 5.39011L7.12 1.39011C7.38 1.21011 7.72001 1.2001 7.98001 1.3801L12.42 4.3801C12.62 4.5201 12.75 4.75008 12.75 4.99008C12.75 5.24008 12.64 5.47008 12.44 5.61008L6.88 9.61008C6.75 9.70008 6.6 9.75009 6.44 9.75009ZM3.31 5.98011L6.42999 8.09009L10.69 5.02008L7.57001 2.9101L3.31 5.98011Z" fill="{color}"/>
<path d="M17.5596 9.75017C17.4096 9.75017 17.2496 9.70016 17.1196 9.61016L11.5596 5.61016C11.3596 5.47016 11.2396 5.23016 11.2496 4.99016C11.2496 4.74016 11.3796 4.52018 11.5796 4.38018L16.0196 1.38018C16.2796 1.21018 16.6196 1.21019 16.8796 1.39019L22.4396 5.39019C22.6396 5.53019 22.7596 5.77018 22.7496 6.01018C22.7496 6.26018 22.6196 6.48017 22.4196 6.62017L17.9796 9.62017C17.8496 9.71017 17.6996 9.75017 17.5596 9.75017ZM13.3096 5.02016L17.5696 8.09017L20.6896 5.98018L16.4296 2.91018L13.3096 5.02016Z" fill="{color}"/>
<path d="M7.5596 17.7502C7.4096 17.7502 7.2496 17.7002 7.1196 17.6102L1.5596 13.6102C1.3596 13.4702 1.2396 13.2302 1.2496 12.9902C1.2496 12.7402 1.37959 12.5202 1.57959 12.3802L6.01959 9.38018C6.27959 9.21018 6.61961 9.21019 6.87961 9.39019L12.4396 13.3902C12.6396 13.5302 12.7596 13.7702 12.7496 14.0102C12.7496 14.2602 12.6196 14.4802 12.4196 14.6202L7.97961 17.6202C7.84961 17.7102 7.6996 17.7502 7.5596 17.7502ZM3.3096 13.0202L7.56961 16.0902L10.6896 13.9802L6.4296 10.9102L3.3096 13.0202Z" fill="{color}"/>
<path d="M16.44 17.7501C16.29 17.7501 16.15 17.7101 16.02 17.6201L11.58 14.6201C11.38 14.4801 11.25 14.2501 11.25 14.0101C11.25 13.7601 11.36 13.5301 11.56 13.3901L17.12 9.39011C17.37 9.21011 17.72 9.2001 17.98 9.3801L22.42 12.3801C22.62 12.5201 22.75 12.7501 22.75 12.9901C22.75 13.2401 22.64 13.4701 22.44 13.6101L16.88 17.6101C16.75 17.7001 16.6 17.7501 16.44 17.7501ZM13.31 13.9801L16.43 16.0901L20.69 13.0201L17.57 10.9101L13.31 13.9801Z" fill="{color}"/>
<path d="M12 22.65C11.75 22.65 11.5 22.6 11.27 22.49L4.69 19.45C4.42 19.33 4.25 19.06 4.25 18.77V15.5C4.25 15.09 4.59 14.75 5 14.75C5.41 14.75 5.75 15.09 5.75 15.5V18.29L11.9 21.13C11.97 21.16 12.04 21.16 12.11 21.13L18.26 18.29V15.5C18.26 15.09 18.6 14.75 19.01 14.75C19.42 14.75 19.76 15.09 19.76 15.5V18.77C19.76 19.06 19.59 19.33 19.32 19.45L12.74 22.49C12.5 22.6 12.25 22.65 12 22.65Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 5L7.56 2L2 6L6.44 9L12 5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 5L16.44 2L22 6L17.56 9L12 5Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 14L7.56 17L2 13L6.44 10L12 14Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 14L16.44 17L22 13L17.56 10L12 14Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M19 15.5V18.77L12.42 21.81C12.15 21.93 11.85 21.93 11.58 21.81L5 18.77V15.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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