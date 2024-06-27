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
<path d="M9 8.38086H13.6846C14.7231 8.38086 15.5654 9.31548 15.5654 10.2616C15.5654 11.3001 14.7231 12.1424 13.6846 12.1424H9V8.38086Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9 12.1309H14.3539C15.5423 12.1309 16.5 12.9732 16.5 14.0116C16.5 15.0501 15.5423 15.8924 14.3539 15.8924H9V12.1309Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12.2769 15.8809V17.7616" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9.93457 15.8809V17.7616" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12.2769 6.5V8.38077" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9.93457 6.5V8.38077" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10.7769 8.38086H7.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10.7769 15.8809H7.5" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M14.9693 12.75H14.1993H9.5293V15.58H10.8393H14.9693C15.9193 15.58 16.6993 14.94 16.6993 14.16C16.6993 13.38 15.9193 12.75 14.9693 12.75Z" fill="{color}"/>
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM14.97 17.08H13.32V18.5C13.32 18.91 12.98 19.25 12.57 19.25C12.16 19.25 11.82 18.91 11.82 18.5V17.08H10.84H10.61V18.5C10.61 18.91 10.27 19.25 9.86 19.25C9.45 19.25 9.11 18.91 9.11 18.5V17.08H8.78H7.05C6.64 17.08 6.3 16.74 6.3 16.33C6.3 15.92 6.64 15.58 7.05 15.58H8.03V12V8.42H7.05C6.64 8.42 6.3 8.08 6.3 7.67C6.3 7.26 6.64 6.92 7.05 6.92H8.78H9.11V5.5C9.11 5.09 9.45 4.75 9.86 4.75C10.27 4.75 10.61 5.09 10.61 5.5V6.92H10.84H11.82V5.5C11.82 5.09 12.16 4.75 12.57 4.75C12.98 4.75 13.32 5.09 13.32 5.5V6.92H14.2C15.75 6.92 17.12 8.28 17.12 9.84C17.12 10.51 16.88 11.12 16.5 11.62C17.51 12.11 18.2 13.07 18.2 14.18C18.2 15.77 16.75 17.08 14.97 17.08Z" fill="{color}"/>
<path d="M15.6193 9.83016C15.6193 9.17016 14.9993 8.41016 14.1993 8.41016H10.8393H9.5293V11.2402H14.1993C14.9793 11.2502 15.6193 10.6102 15.6193 9.83016Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M8.7793 7.66992H14.1993C15.3993 7.66992 16.3693 8.74992 16.3693 9.83992C16.3693 11.0399 15.3993 12.0099 14.1993 12.0099H8.7793V7.66992Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.7793 12H14.9693C16.3393 12 17.4493 12.97 17.4493 14.17C17.4493 15.37 16.3393 16.34 14.9693 16.34H8.7793V12Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12.5703 16.3301V18.5001" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9.86914 16.3301V18.5001" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12.5703 5.5V7.67" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9.86914 5.5V7.67" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10.8408 7.66992H7.05078" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10.8408 16.3301H7.05078" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.2 2.3 7.97 2.85" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M21.988 15.48c0.507-0.653 0.827-1.48 0.827-2.373 0-2.067-1.813-3.893-3.893-3.893h-1.173v-1.88c0-0.547-0.453-1-1-1s-1 0.453-1 1v1.893h-1.613v-1.893c0-0.547-0.453-1-1-1s-0.973 0.453-0.973 1v1.893h-2.76c-0.547 0-1 0.453-1 1s0.453 1 1 1h1.307v9.547h-1.307c-0.547 0-1 0.453-1 1s0.453 1 1 1h2.747v1.893c0 0.547 0.453 1 1 1s1-0.453 1-1v-1.893h1.613v1.893c0 0.547 0.453 1 1 1s1-0.453 1-1v-1.893h2.2c2.373 0 4.307-1.747 4.307-3.893 0-1.467-0.933-2.747-2.28-3.4zM14.454 11.227h4.48c1.067 0 1.893 1.013 1.893 1.893 0 1.040-0.853 1.893-1.893 1.893h-6.227v-3.787h1.747zM19.961 20.773h-7.253v-3.773h7.253c1.267 0 2.307 0.853 2.307 1.893s-1.040 1.88-2.307 1.88z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
<path d="M14.2003 12.7499H8.78027C8.37027 12.7499 8.03027 12.4099 8.03027 11.9999V7.66992C8.03027 7.25992 8.37027 6.91992 8.78027 6.91992H14.2003C15.7503 6.91992 17.1203 8.27992 17.1203 9.83992C17.1203 11.4399 15.8103 12.7499 14.2003 12.7499ZM9.53027 11.2499H14.2003C14.9803 11.2499 15.6203 10.6099 15.6203 9.82992C15.6203 9.16992 15.0003 8.40992 14.2003 8.40992H9.53027V11.2499Z" fill="{color}"/>
<path d="M14.9703 17.08H8.78027C8.37027 17.08 8.03027 16.74 8.03027 16.33V12C8.03027 11.59 8.37027 11.25 8.78027 11.25H14.9703C16.7503 11.25 18.2003 12.56 18.2003 14.17C18.2003 15.78 16.7503 17.08 14.9703 17.08ZM9.53027 15.58H14.9703C15.9203 15.58 16.7003 14.94 16.7003 14.16C16.7003 13.38 15.9303 12.74 14.9703 12.74H9.53027V15.58Z" fill="{color}"/>
<path d="M12.5703 19.2501C12.1603 19.2501 11.8203 18.9101 11.8203 18.5001V16.3301C11.8203 15.9201 12.1603 15.5801 12.5703 15.5801C12.9803 15.5801 13.3203 15.9201 13.3203 16.3301V18.5001C13.3203 18.9101 12.9903 19.2501 12.5703 19.2501Z" fill="{color}"/>
<path d="M9.87012 19.2501C9.46012 19.2501 9.12012 18.9101 9.12012 18.5001V16.3301C9.12012 15.9201 9.46012 15.5801 9.87012 15.5801C10.2801 15.5801 10.6201 15.9201 10.6201 16.3301V18.5001C10.6201 18.9101 10.2801 19.2501 9.87012 19.2501Z" fill="{color}"/>
<path d="M12.5703 8.42C12.1603 8.42 11.8203 8.08 11.8203 7.67V5.5C11.8203 5.09 12.1603 4.75 12.5703 4.75C12.9803 4.75 13.3203 5.09 13.3203 5.5V7.67C13.3203 8.08 12.9903 8.42 12.5703 8.42Z" fill="{color}"/>
<path d="M9.87012 8.42C9.46012 8.42 9.12012 8.08 9.12012 7.67V5.5C9.12012 5.09 9.46012 4.75 9.87012 4.75C10.2801 4.75 10.6201 5.09 10.6201 5.5V7.67C10.6201 8.08 10.2801 8.42 9.87012 8.42Z" fill="{color}"/>
<path d="M10.8398 8.41992H7.0498C6.6398 8.41992 6.2998 8.07992 6.2998 7.66992C6.2998 7.25992 6.6398 6.91992 7.0498 6.91992H10.8398C11.2498 6.91992 11.5898 7.25992 11.5898 7.66992C11.5898 8.07992 11.2598 8.41992 10.8398 8.41992Z" fill="{color}"/>
<path d="M10.8398 17.0801H7.0498C6.6398 17.0801 6.2998 16.7401 6.2998 16.3301C6.2998 15.9201 6.6398 15.5801 7.0498 15.5801H10.8398C11.2498 15.5801 11.5898 15.9201 11.5898 16.3301C11.5898 16.7401 11.2598 17.0801 10.8398 17.0801Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<g opacity="0.4">
<path d="M8.7793 7.66992H14.1993C15.3993 7.66992 16.3693 8.74992 16.3693 9.83992C16.3693 11.0399 15.3993 12.0099 14.1993 12.0099H8.7793V7.66992Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.7793 12H14.9693C16.3393 12 17.4493 12.97 17.4493 14.17C17.4493 15.37 16.3393 16.34 14.9693 16.34H8.7793V12Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12.5703 16.3301V18.5001" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9.87012 16.3301V18.5001" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12.5703 5.5V7.67" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9.87012 5.5V7.67" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10.8398 7.66992H7.0498" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10.8398 16.3301H7.0498" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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