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
<path d="M9 22H15C20 22 22 20 22 15V9C22 4 20 2 15 2H9C4 2 2 4 2 9V15C2 20 4 22 9 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10 17H14C15.65 17 17 15.65 17 14V10C17 8.35 15.65 7 14 7H10C8.35 7 7 8.35 7 10V14C7 15.65 8.35 17 10 17Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 7V17" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7 12H17" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M8.05078 10.1408V11.3008H11.3108V8.05078H10.1508C8.99078 8.05078 8.05078 8.99078 8.05078 10.1408Z" fill="{color}"/>
<path d="M8.05078 13.8592C8.05078 15.0092 8.99078 15.9492 10.1408 15.9492H11.3008V12.6992H8.05078V13.8592Z" fill="{color}"/>
<path d="M12.6992 15.9492H13.8592C15.0092 15.9492 15.9492 15.0092 15.9492 13.8592V12.6992H12.6992V15.9492Z" fill="{color}"/>
<path d="M16.19 2H7.81C4.17 2 2 4.17 2 7.81V16.18C2 19.83 4.17 22 7.81 22H16.18C19.82 22 21.99 19.83 21.99 16.19V7.81C22 4.17 19.83 2 16.19 2ZM17.35 13.86C17.35 15.78 15.78 17.35 13.86 17.35H10.14C8.22 17.35 6.65 15.79 6.65 13.86V10.14C6.65 8.22 8.22 6.65 10.14 6.65H13.86C15.78 6.65 17.35 8.21 17.35 10.14V13.86Z" fill="{color}"/>
<path d="M13.8592 8.05078H12.6992V11.3108H15.9592V10.1508C15.9492 8.99078 15.0092 8.05078 13.8592 8.05078Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M14 7H10C8.35 7 7 8.35 7 10V14C7 15.65 8.35 17 10 17H14C15.65 17 17 15.65 17 14V10" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 7V17" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7 12H17" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2 12.98V15C2 20 4 22 9 22H15C20 22 22 20 22 15V9C22 4 20 2 15 2H9C4 2 2 4 2 9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M16.19 2H7.81C4.17 2 2 4.17 2 7.81V16.18C2 19.83 4.17 22 7.81 22H16.18C19.82 22 21.99 19.83 21.99 16.19V7.81C22 4.17 19.83 2 16.19 2Z" fill="{color}"/>
<path d="M13.8604 6.6499H10.1404C8.22039 6.6499 6.65039 8.2099 6.65039 10.1399V13.8599C6.65039 15.7799 8.22039 17.3499 10.1404 17.3499H13.8604C15.7804 17.3499 17.3504 15.7899 17.3504 13.8599V10.1399C17.3504 8.2199 15.7804 6.6499 13.8604 6.6499ZM15.9504 10.1399V11.2999H12.7004V8.0499H13.8604C15.0104 8.0499 15.9504 8.9899 15.9504 10.1399ZM10.1404 8.0499H11.3004V11.3099H8.05039V10.1499C8.05039 8.9899 8.99039 8.0499 10.1404 8.0499ZM8.05039 13.8599V12.6999H11.3104V15.9599H10.1504C8.99039 15.9499 8.05039 15.0099 8.05039 13.8599ZM13.8604 15.9499H12.7004V12.6999H15.9604V13.8599C15.9504 15.0099 15.0104 15.9499 13.8604 15.9499Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15 22.75H9C3.57 22.75 1.25 20.43 1.25 15V9C1.25 3.57 3.57 1.25 9 1.25H15C20.43 1.25 22.75 3.57 22.75 9V15C22.75 20.43 20.43 22.75 15 22.75ZM9 2.75C4.39 2.75 2.75 4.39 2.75 9V15C2.75 19.61 4.39 21.25 9 21.25H15C19.61 21.25 21.25 19.61 21.25 15V9C21.25 4.39 19.61 2.75 15 2.75H9Z" fill="{color}"/>
<path d="M14 17.75H10C7.93 17.75 6.25 16.07 6.25 14V10C6.25 7.93 7.93 6.25 10 6.25H14C16.07 6.25 17.75 7.93 17.75 10V14C17.75 16.07 16.07 17.75 14 17.75ZM10 7.75C8.76 7.75 7.75 8.76 7.75 10V14C7.75 15.24 8.76 16.25 10 16.25H14C15.24 16.25 16.25 15.24 16.25 14V10C16.25 8.76 15.24 7.75 14 7.75H10Z" fill="{color}"/>
<path d="M12 17.75C11.59 17.75 11.25 17.41 11.25 17V7C11.25 6.59 11.59 6.25 12 6.25C12.41 6.25 12.75 6.59 12.75 7V17C12.75 17.41 12.41 17.75 12 17.75Z" fill="{color}"/>
<path d="M17 12.75H7C6.59 12.75 6.25 12.41 6.25 12C6.25 11.59 6.59 11.25 7 11.25H17C17.41 11.25 17.75 11.59 17.75 12C17.75 12.41 17.41 12.75 17 12.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M9 22H15C20 22 22 20 22 15V9C22 4 20 2 15 2H9C4 2 2 4 2 9V15C2 20 4 22 9 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<g opacity="0.4">
<path d="M10 17H14C15.65 17 17 15.65 17 14V10C17 8.35 15.65 7 14 7H10C8.35 7 7 8.35 7 10V14C7 15.65 8.35 17 10 17Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 7V17" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7 12H17" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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