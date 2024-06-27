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
<path d="M6.69995 16L10.2 8L13.8 16" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7.5 13.3H12.9" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path d="M16.3 16V10.7" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15 22H9C4 22 2 20 2 15V9C2 4 4 2 9 2H15C20 2 22 4 22 9V15C22 20 20 22 15 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16.3401 8.03418V8.03418" stroke="{color}" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.19 2H7.81C4.17 2 2 4.17 2 7.81V16.18C2 19.82 4.17 21.99 7.81 21.99H16.18C19.82 21.99 21.99 19.82 21.99 16.18V7.81C22 4.17 19.83 2 16.19 2ZM13.06 16.68C12.98 16.71 12.9 16.72 12.82 16.72C12.51 16.72 12.21 16.52 12.11 16.21L11.4 14.08H8.32L7.34 16.28C7.17 16.66 6.73 16.83 6.35 16.66C5.97 16.49 5.8 16.05 5.97 15.67L9.5 7.73999C9.63 7.45999 9.9 7.26999 10.22 7.29999C10.53 7.30999 10.8 7.52 10.9 7.81L13.54 15.74C13.66 16.12 13.45 16.55 13.06 16.68ZM17.1 15.97C17.1 16.38 16.76 16.72 16.35 16.72C15.94 16.72 15.6 16.38 15.6 15.97V10.68C15.6 10.27 15.94 9.92999 16.35 9.92999C16.76 9.92999 17.1 10.27 17.1 10.68V15.97ZM17.27 8.42001C17.22 8.54001 17.15 8.64999 17.05 8.73999C16.96 8.82999 16.85 8.90999 16.73 8.95999C16.61 9.00999 16.48 9.03 16.35 9.03C16.08 9.03 15.83 8.92999 15.64 8.73999C15.55 8.64999 15.47 8.54001 15.42 8.42001C15.37 8.29001 15.35 8.17 15.35 8.03C15.35 7.9 15.37 7.76999 15.42 7.64999C15.48 7.52999 15.55 7.41999 15.64 7.32999C15.73 7.22999 15.84 7.15999 15.96 7.10999C16.33 6.95999 16.78 7.04999 17.05 7.32999C17.15 7.41999 17.22 7.52999 17.27 7.64999C17.32 7.76999 17.35 7.9 17.35 8.03C17.35 8.17 17.32 8.30001 17.27 8.42001Z" fill="{color}"/>
<path d="M8.98047 12.5694H10.9005L10.0805 10.1094L8.98047 12.5694Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.25 8V8" stroke="{color}" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6.65039 15.97L10.1804 8.03003L12.8204 15.97" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7.5293 13.3201H11.9393" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path d="M16.3496 15.9699V10.6799" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 12.83V15C2 20 4 22 9 22H15C20 22 22 20 22 15V9C22 4 20 2 15 2H9C4 2 2 4 2 9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M21.587 2.667h-11.173c-4.853 0-7.747 2.893-7.747 7.747v11.16c0 4.853 2.893 7.747 7.747 7.747h11.16c4.853 0 7.747-2.893 7.747-7.747v-11.16c0.013-4.853-2.88-7.747-7.733-7.747z"></path>
<path fill="{color}" d="M14.521 10.4c-0.133-0.387-0.493-0.667-0.907-0.68-0.427-0.027-0.8 0.213-0.96 0.587l-4.707 10.573c-0.227 0.507 0 1.093 0.507 1.32s1.093 0 1.32-0.507l1.307-2.933h4.107l0.947 2.84c0.133 0.413 0.533 0.68 0.947 0.68 0.107 0 0.213-0.013 0.32-0.053 0.52-0.173 0.8-0.747 0.627-1.267l-3.507-10.56zM11.974 16.76l1.467-3.293 1.093 3.293h-2.56z"></path>
<path fill="{color}" d="M21.799 13.24c-0.547 0-1 0.453-1 1v7.053c0 0.547 0.453 1 1 1s1-0.453 1-1v-7.053c0-0.56-0.453-1-1-1z"></path>
<path fill="{color}" d="M23.026 10.2c-0.067-0.16-0.16-0.307-0.293-0.427-0.36-0.373-0.96-0.493-1.453-0.293-0.16 0.067-0.307 0.16-0.427 0.293-0.12 0.12-0.213 0.267-0.293 0.427-0.067 0.16-0.093 0.333-0.093 0.507 0 0.187 0.027 0.347 0.093 0.52 0.067 0.16 0.173 0.307 0.293 0.427 0.253 0.253 0.587 0.387 0.947 0.387 0.173 0 0.347-0.027 0.507-0.093s0.307-0.173 0.427-0.293c0.133-0.12 0.227-0.267 0.293-0.427s0.107-0.333 0.107-0.52c0-0.173-0.040-0.347-0.107-0.507z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12.8202 16.72C12.5102 16.72 12.2102 16.52 12.1102 16.21L10.0802 10.11L7.34024 16.28C7.17024 16.66 6.73024 16.83 6.35024 16.66C5.97024 16.49 5.80024 16.05 5.97024 15.67L9.50024 7.73999C9.63024 7.45999 9.90024 7.26999 10.2202 7.29999C10.5302 7.30999 10.8002 7.52 10.9002 7.81L13.5402 15.74C13.6702 16.13 13.4602 16.56 13.0702 16.69C12.9802 16.7 12.9002 16.72 12.8202 16.72Z" fill="{color}"/>
<path d="M11.9403 12.5698H7.53027V14.0698H11.9403V12.5698Z" fill="{color}"/>
<path d="M16.3496 16.7202C15.9396 16.7202 15.5996 16.3802 15.5996 15.9702V10.6802C15.5996 10.2702 15.9396 9.93018 16.3496 9.93018C16.7596 9.93018 17.0996 10.2702 17.0996 10.6802V15.9702C17.0996 16.3802 16.7596 16.7202 16.3496 16.7202Z" fill="{color}"/>
<path d="M16.3496 9.03002C16.0796 9.03002 15.8296 8.93001 15.6396 8.74001C15.5496 8.65001 15.4696 8.54003 15.4196 8.42003C15.3696 8.29003 15.3496 8.17002 15.3496 8.03002C15.3496 7.90002 15.3696 7.77001 15.4196 7.65001C15.4796 7.53001 15.5496 7.42 15.6396 7.33C15.7296 7.23 15.8396 7.16 15.9596 7.11C16.3296 6.96 16.7796 7.05 17.0496 7.33C17.1496 7.42 17.2196 7.53001 17.2696 7.65001C17.3196 7.77001 17.3496 7.90002 17.3496 8.03002C17.3496 8.17002 17.3196 8.30003 17.2696 8.42003C17.2196 8.54003 17.1496 8.65001 17.0496 8.74001C16.9596 8.83001 16.8496 8.91001 16.7296 8.96001C16.6096 9.01001 16.4796 9.03002 16.3496 9.03002Z" fill="{color}"/>
<path d="M15 22.75H9C3.57 22.75 1.25 20.43 1.25 15V9C1.25 3.57 3.57 1.25 9 1.25H15C20.43 1.25 22.75 3.57 22.75 9V15C22.75 20.43 20.43 22.75 15 22.75ZM9 2.75C4.39 2.75 2.75 4.39 2.75 9V15C2.75 19.61 4.39 21.25 9 21.25H15C19.61 21.25 21.25 19.61 21.25 15V9C21.25 4.39 19.61 2.75 15 2.75H9Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15 22H9C4 22 2 20 2 15V9C2 4 4 2 9 2H15C20 2 22 4 22 9V15C22 20 20 22 15 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<g opacity="0.4">
<path d="M6.5 16L10 8L13.6 16" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7.2998 13.2998H12.6998" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
<path d="M16.0996 16.0002V10.7002" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16.1406 8.03418V8.03418" stroke="{color}" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
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