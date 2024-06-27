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
<path d="M17 3.30005H7L2 12L7 20.7001H17L22 12L17 3.30005Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path d="M10.9001 14H7.0001L5.1001 17.3L7.0001 20.7H10.9001L12.8001 17.3L10.9001 14Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path d="M14.2999 8H6.9999L3.3999 14.3L6.9999 20.7H14.2999L17.9999 14.3L14.2999 8Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.13" d="M10.8698 14L12.7998 17.33L10.8799 20.66H6.99985L5.08984 17.35L7.02985 14H10.8698Z" fill="{color}"/>
<path d="M10.5396 14.0781H7.11959C6.93959 14.0781 6.7796 14.1781 6.6896 14.3281L4.97961 17.2881C4.88961 17.4381 4.88961 17.6381 4.97961 17.7881L6.6896 20.7481C6.7796 20.8981 6.93959 20.9981 7.11959 20.9981H10.5396C10.7196 20.9981 10.8796 20.8981 10.9696 20.7481L12.6796 17.7881C12.7696 17.6381 12.7696 17.4381 12.6796 17.2881L10.9696 14.3281C10.8796 14.1681 10.7196 14.0781 10.5396 14.0781Z" fill="{color}"/>
<path d="M22.2401 11.7383C22.3301 11.8983 22.3301 12.0983 22.2401 12.2583L17.3102 20.7883C17.2402 20.9183 17.1002 20.9983 16.9502 20.9983C16.6302 20.9983 16.4302 20.6483 16.5902 20.3783L19.8802 14.6783C19.9702 14.5183 19.9702 14.3183 19.8802 14.1583L15.4802 6.53828C15.3902 6.37828 15.2202 6.27828 15.0302 6.27828H6.22016C6.03016 6.27828 5.87014 6.37828 5.77014 6.53828L2.50016 12.2183C2.33016 12.5183 1.90016 12.5183 1.72016 12.2183C1.64016 12.0783 1.64016 11.9083 1.72016 11.7683L6.64017 3.24828C6.72017 3.08828 6.90015 2.98828 7.09015 2.98828H16.8802C17.0702 2.98828 17.2301 3.08828 17.3301 3.24828L22.2401 11.7383Z" fill="{color}"/>
<path d="M18.089 14.6816L14.589 20.7416C14.499 20.9016 14.3291 21.0016 14.1391 21.0016H13.5391C13.1391 21.0016 12.889 20.5716 13.089 20.2216L14.489 17.8016C14.579 17.6416 14.579 17.4416 14.489 17.2816L11.8891 12.7816C11.7891 12.6216 11.6091 12.5216 11.4191 12.5216H6.21905C6.02905 12.5216 5.86904 12.6216 5.76904 12.7816L4.36904 15.2016C4.16904 15.5516 3.66905 15.5516 3.46905 15.2016L3.16906 14.6916C3.07906 14.5316 3.07906 14.3316 3.16906 14.1716L6.65905 8.11156C6.74905 7.95156 6.91903 7.85156 7.10903 7.85156H14.0991C14.2891 7.85156 14.449 7.95156 14.549 8.11156L18.049 14.1716C18.169 14.3216 18.169 14.5316 18.089 14.6816Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M4.51001 7.65009L2 12.0001L7 20.6601H17L22 12.0001L17 3.34009H7L6.63 3.98009" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10.8696 14H7.0296L5.09961 17.33L7.0296 20.66H10.8696L12.7996 17.33L10.8696 14Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
<path d="M14.3409 8H7.03085L3.38086 14.33L7.03085 20.66H14.3409L18.0009 14.33L14.3409 8Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M22.667 4.453h-13.333l-6.667 11.547 6.667 11.547h13.333l6.667-11.547-6.667-11.547z"></path>
<path fill="{color}" d="M14.493 18.667h-5.12l-2.573 4.44 2.573 4.44h5.12l2.573-4.44-2.573-4.44z"></path>
<path fill="{color}" opacity="0.6" d="M19.121 10.667h-9.747l-4.867 8.44 4.867 8.44h9.747l4.88-8.44-4.88-8.44z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M17.4299 21.4099H6.55988L1.12988 11.9998L6.55988 2.58984H17.4299L22.8599 11.9998L17.4299 21.4099ZM7.42987 19.9099H16.5599L21.1299 11.9998L16.5599 4.08984H7.42987L2.86987 11.9998L7.42987 19.9099Z" fill="{color}"/>
<path d="M11.3102 21.41H6.60025L4.24023 17.33L6.60025 13.25H11.3102L13.6703 17.33L11.3102 21.41ZM7.46024 19.91H10.4402L11.9302 17.33L10.4402 14.75H7.46024L5.97025 17.33L7.46024 19.91Z" fill="{color}"/>
<path d="M14.7798 21.41H6.59976L2.50977 14.33L6.59976 7.25H14.7798L18.8698 14.33L14.7798 21.41ZM7.46976 19.91H13.9098L17.1298 14.33L13.9098 8.75H7.46976L4.24976 14.33L7.46976 19.91Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M17 3.33984H7L2 11.9998L7 20.6599H17L22 11.9998L17 3.33984Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path opacity="0.4" d="M10.8696 14H7.0296L5.09961 17.33L7.0296 20.66H10.8696L12.7996 17.33L10.8696 14Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path opacity="0.4" d="M14.3399 8H7.02988L3.37988 14.33L7.02988 20.66H14.3399L17.9999 14.33L14.3399 8Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
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