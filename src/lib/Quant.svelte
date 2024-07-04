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
<path d="M12 2L3 7V17L12 22L17 19.5L21 22V17L17 14.8L21 12V7L12 2Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 6.3999L7 9.1999V14.7999L12 17.5999L17 14.7999V9.1999L12 6.3999Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3 7L7 9.2" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3 17L7 14.8" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M21 7L17 9.2" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 6V2" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22V18" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17 20V15" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M20.4897 6.70813L12.4897 2.26812C12.1897 2.09812 11.8198 2.09812 11.5198 2.26812L3.51978 6.70813C3.19978 6.88813 3.00977 7.21812 3.00977 7.57812V16.3981C3.00977 16.7581 3.20978 17.0981 3.51978 17.2681L11.5397 21.7281C11.8297 21.8881 12.1797 21.8981 12.4697 21.7481L16.4998 19.7381C16.8098 19.5781 17.1797 19.5981 17.4797 19.7881L19.4697 21.0381C20.1397 21.4581 20.9998 20.9781 20.9998 20.1881V17.5781C20.9998 17.2181 20.7997 16.8781 20.4897 16.7081L17.4897 15.0481C17.1897 14.8781 16.8198 14.8781 16.5198 15.0481L12.4897 17.2881C12.1897 17.4581 11.8198 17.4581 11.5198 17.2881L7.51978 15.0681C7.19978 14.8881 7.00977 14.5581 7.00977 14.1981V9.81813C7.00977 9.45813 7.20978 9.11812 7.51978 8.94812L11.5198 6.72812C11.8198 6.55812 12.1897 6.55812 12.4897 6.72812L16.4897 8.94812C16.8097 9.12812 16.9998 9.45813 16.9998 9.81813V12.8781C16.9998 13.6881 17.9098 14.1581 18.5698 13.6981L20.5698 12.3081C20.8398 12.1181 20.9998 11.8181 20.9998 11.4881V7.59813C20.9998 7.22813 20.7997 6.88813 20.4897 6.70813Z" fill="{color}"/>
<path d="M15.8606 10.4216V13.5716C15.8606 13.9216 15.6706 14.2416 15.3606 14.4116L12.4706 16.0216C12.1806 16.1816 11.8206 16.1816 11.5306 16.0216L8.64062 14.4116C8.33062 14.2416 8.14062 13.9216 8.14062 13.5716V10.4216C8.14062 10.0716 8.33062 9.75156 8.64062 9.58156L11.5306 7.97156C11.8206 7.81156 12.1806 7.81156 12.4706 7.97156L15.3606 9.58156C15.6706 9.75156 15.8606 10.0716 15.8606 10.4216Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M6.25 5.19L3 7V17L12 22L17 19.5L21 22V17L17 14.78L21 12V7L12 2L9.96002 3.13" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 6.43994L7 9.21994V14.7799L12 17.5599L17 14.7799V9.21994L12 6.43994Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3 7L7 9.23" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3 17L7 14.77" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M21 7L17 9.23" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 6V2" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22V18" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17 20V15" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.6" d="M28 9.333v6.667l-5.333 3.707v-7.4l5.333-2.973z"></path>
<path fill="{color}" opacity="0.6" d="M16 23.413v5.92l-12-6.667 5.333-2.973v0.013l6.667 3.707z"></path>
<path fill="{color}" d="M9.333 12.307v7.387l-5.333 2.973v-13.333l5.333 2.973z"></path>
<path fill="{color}" opacity="0.6" d="M16 2.667v5.92l-6.667 3.707v0.013l-5.333-2.973 12-6.667z"></path>
<path fill="{color}" d="M22.667 12.307v-0.013l-6.667-3.707v-5.92l12 6.667-5.333 2.973z"></path>
<path fill="{color}" d="M22.667 19.707v6.293l-6.667 3.333v-5.92l6.667-3.707z"></path>
<path fill="{color}" opacity="0.4" d="M28 22.667v6.667l-5.333-3.333v-6.293l5.333 2.96z"></path>
<path fill="{color}" opacity="0.4" d="M22.667 12.293v7.413l-6.667 3.707-6.667-3.707v-7.413l6.667-3.707 6.667 3.707z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22.7502C11.87 22.7502 11.75 22.7202 11.64 22.6602L2.64001 17.6602C2.40001 17.5302 2.25 17.2802 2.25 17.0002V7.00018C2.25 6.73018 2.40001 6.48018 2.64001 6.34018L11.64 1.34018C11.87 1.21018 12.14 1.21018 12.37 1.34018L21.37 6.34018C21.61 6.47018 21.76 6.72018 21.76 7.00018V12.0002C21.76 12.2502 21.64 12.4802 21.44 12.6202L18.43 14.7102L21.38 16.3502C21.62 16.4802 21.77 16.7302 21.77 17.0102V22.0102C21.77 22.2802 21.62 22.5302 21.38 22.6702C21.14 22.8002 20.85 22.8002 20.62 22.6502L16.98 20.3702L12.36 22.6802C12.23 22.7202 12.12 22.7502 12 22.7502ZM3.75 16.5602L12.02 21.1502L16.67 18.8302C16.9 18.7102 17.18 18.7302 17.4 18.8602L20.25 20.6402V17.4302L16.64 15.4202C16.41 15.2902 16.27 15.0602 16.26 14.8002C16.25 14.5402 16.37 14.2902 16.58 14.1502L20.26 11.6002V7.43017L12.01 2.85019L3.76001 7.43017V16.5602H3.75Z" fill="{color}"/>
<path d="M12 18.3101C11.87 18.3101 11.75 18.2801 11.64 18.2201L6.64001 15.4401C6.40001 15.3101 6.25 15.0601 6.25 14.7801V9.22012C6.25 8.95012 6.40001 8.70012 6.64001 8.56012L11.64 5.78012C11.87 5.65012 12.14 5.65012 12.37 5.78012L17.37 8.56012C17.61 8.69012 17.76 8.94012 17.76 9.22012V14.7801C17.76 15.0501 17.61 15.3001 17.37 15.4401L12.37 18.2201C12.25 18.2701 12.13 18.3101 12 18.3101ZM7.75 14.3401L12 16.7001L16.25 14.3401V9.67012L12 7.30012L7.75 9.66012V14.3401Z" fill="{color}"/>
<path d="M6.99978 9.97975C6.87978 9.97975 6.74979 9.94976 6.63979 9.88976L2.63979 7.65976C2.27979 7.45976 2.14975 6.99976 2.34975 6.63976C2.54975 6.27976 2.99977 6.14976 3.36977 6.34976L7.36977 8.57976C7.72977 8.77976 7.85975 9.23976 7.65975 9.59976C7.50975 9.83976 7.25978 9.97975 6.99978 9.97975Z" fill="{color}"/>
<path d="M2.99998 17.75C2.73998 17.75 2.48 17.61 2.34 17.36C2.14 17 2.26998 16.54 2.62998 16.34L6.62998 14.11C6.99998 13.91 7.45 14.04 7.65 14.4C7.85 14.76 7.71996 15.22 7.35996 15.42L3.35996 17.65C3.24996 17.72 3.11998 17.75 2.99998 17.75Z" fill="{color}"/>
<path d="M17 9.97999C16.74 9.97999 16.48 9.83999 16.34 9.58999C16.14 9.22999 16.27 8.77001 16.63 8.57001L20.63 6.33999C21 6.13999 21.45 6.27 21.65 6.63C21.85 6.99 21.72 7.44999 21.36 7.64999L17.36 9.88C17.25 9.95 17.13 9.97999 17 9.97999Z" fill="{color}"/>
<path d="M12 6.75C11.59 6.75 11.25 6.41 11.25 6V2C11.25 1.59 11.59 1.25 12 1.25C12.41 1.25 12.75 1.59 12.75 2V6C12.75 6.41 12.41 6.75 12 6.75Z" fill="{color}"/>
<path d="M12 22.75C11.59 22.75 11.25 22.41 11.25 22V18C11.25 17.59 11.59 17.25 12 17.25C12.41 17.25 12.75 17.59 12.75 18V22C12.75 22.41 12.41 22.75 12 22.75Z" fill="{color}"/>
<path d="M17.75 15H16.25V20H17.75V15Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 6.43994L7 9.21994V14.7799L12 17.5599L17 14.7799V9.21994L12 6.43994Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<g opacity="0.4">
<path d="M12 2L3 7V17L12 22L17 19.5L21 22V17L17 14.78L21 12V7L12 2Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3 7L7 9.23" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3 17L7 14.77" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M21 7L17 9.23" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 6V2" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22V18" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17 20V15" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
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
	.horizontal-reverted {
		transform: scale(-1, 1);
	}
	.vertical-reverted {
		transform: scale(1, -1);
	}
</style>