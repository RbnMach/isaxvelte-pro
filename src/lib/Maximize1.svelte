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
<path d="M2 9V6.5C2 4.01 4.01 2 6.5 2H9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15 2H17.5C19.99 2 22 4.01 22 6.5V9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M22 16V17.5C22 19.99 19.99 22 17.5 22H16" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9 22H6.5C4.01 22 2 19.99 2 17.5V15" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M18 12V10M6 12H12H18H6ZM6 12V10V12ZM6 12V14V12ZM18 12V14V12Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 6H14M12 18V6V18ZM12 18H14H12ZM12 18H10H12ZM12 6H10H12Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.19 2H7.81C4.17 2 2 4.17 2 7.81V16.18C2 19.83 4.17 22 7.81 22H16.18C19.82 22 21.99 19.83 21.99 16.19V7.81C22 4.17 19.83 2 16.19 2ZM18.75 14C18.75 14.41 18.41 14.75 18 14.75C17.59 14.75 17.25 14.41 17.25 14V12.75H12.75V17.25H14C14.41 17.25 14.75 17.59 14.75 18C14.75 18.41 14.41 18.75 14 18.75H10C9.59 18.75 9.25 18.41 9.25 18C9.25 17.59 9.59 17.25 10 17.25H11.25V12.75H6.75V14C6.75 14.41 6.41 14.75 6 14.75C5.59 14.75 5.25 14.41 5.25 14V10C5.25 9.59 5.59 9.25 6 9.25C6.41 9.25 6.75 9.59 6.75 10V11.25H11.25V6.75H10C9.59 6.75 9.25 6.41 9.25 6C9.25 5.59 9.59 5.25 10 5.25H14C14.41 5.25 14.75 5.59 14.75 6C14.75 6.41 14.41 6.75 14 6.75H12.75V11.25H17.25V10C17.25 9.59 17.59 9.25 18 9.25C18.41 9.25 18.75 9.59 18.75 10V14Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2 9V6.5C2 4.01 4.01 2 6.5 2H9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15 2H17.5C19.99 2 22 4.01 22 6.5V9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M22 16V17.5C22 19.99 19.99 22 17.5 22H16" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9 22H6.5C4.01 22 2 19.99 2 17.5V15" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M18 12V10M16.95 12H18H16.95ZM6 12H12H14H6ZM6 12V10V12ZM6 12V14V12ZM18 12V14V12Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 6H14M12 18V6V18ZM12 18H14H12ZM12 18H10H12ZM12 6H10H12Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M16.19 2H7.81C4.17 2 2 4.17 2 7.81V16.18C2 19.83 4.17 22 7.81 22H16.18C19.82 22 21.99 19.83 21.99 16.19V7.81C22 4.17 19.83 2 16.19 2Z" fill="{color}"/>
<path d="M18 9.25C17.59 9.25 17.25 9.59 17.25 10V11.25H12.75V6.75H14C14.41 6.75 14.75 6.41 14.75 6C14.75 5.59 14.41 5.25 14 5.25H10C9.59 5.25 9.25 5.59 9.25 6C9.25 6.41 9.59 6.75 10 6.75H11.25V11.25H6.75V10C6.75 9.59 6.41 9.25 6 9.25C5.59 9.25 5.25 9.59 5.25 10V14C5.25 14.41 5.59 14.75 6 14.75C6.41 14.75 6.75 14.41 6.75 14V12.75H11.25V17.25H10C9.59 17.25 9.25 17.59 9.25 18C9.25 18.41 9.59 18.75 10 18.75H14C14.41 18.75 14.75 18.41 14.75 18C14.75 17.59 14.41 17.25 14 17.25H12.75V12.75H17.25V14C17.25 14.41 17.59 14.75 18 14.75C18.41 14.75 18.75 14.41 18.75 14V10C18.75 9.59 18.41 9.25 18 9.25Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2 9.75C1.59 9.75 1.25 9.41 1.25 9V6.5C1.25 3.61 3.61 1.25 6.5 1.25H9C9.41 1.25 9.75 1.59 9.75 2C9.75 2.41 9.41 2.75 9 2.75H6.5C4.43 2.75 2.75 4.43 2.75 6.5V9C2.75 9.41 2.41 9.75 2 9.75Z" fill="{color}"/>
<path d="M22 9.75C21.59 9.75 21.25 9.41 21.25 9V6.5C21.25 4.43 19.57 2.75 17.5 2.75H15C14.59 2.75 14.25 2.41 14.25 2C14.25 1.59 14.59 1.25 15 1.25H17.5C20.39 1.25 22.75 3.61 22.75 6.5V9C22.75 9.41 22.41 9.75 22 9.75Z" fill="{color}"/>
<path d="M17.5 22.75H16C15.59 22.75 15.25 22.41 15.25 22C15.25 21.59 15.59 21.25 16 21.25H17.5C19.57 21.25 21.25 19.57 21.25 17.5V16C21.25 15.59 21.59 15.25 22 15.25C22.41 15.25 22.75 15.59 22.75 16V17.5C22.75 20.39 20.39 22.75 17.5 22.75Z" fill="{color}"/>
<path d="M9 22.75H6.5C3.61 22.75 1.25 20.39 1.25 17.5V15C1.25 14.59 1.59 14.25 2 14.25C2.41 14.25 2.75 14.59 2.75 15V17.5C2.75 19.57 4.43 21.25 6.5 21.25H9C9.41 21.25 9.75 21.59 9.75 22C9.75 22.41 9.41 22.75 9 22.75Z" fill="{color}"/>
<path d="M18 14.75C17.59 14.75 17.25 14.41 17.25 14V12.75H6.75V14C6.75 14.41 6.41 14.75 6 14.75C5.59 14.75 5.25 14.41 5.25 14V10C5.25 9.59 5.59 9.25 6 9.25C6.41 9.25 6.75 9.59 6.75 10V11.25H17.25V10C17.25 9.59 17.59 9.25 18 9.25C18.41 9.25 18.75 9.59 18.75 10V14C18.75 14.41 18.41 14.75 18 14.75Z" fill="{color}"/>
<path d="M14 18.75H10C9.59 18.75 9.25 18.41 9.25 18C9.25 17.59 9.59 17.25 10 17.25H11.25V6.75H10C9.59 6.75 9.25 6.41 9.25 6C9.25 5.59 9.59 5.25 10 5.25H14C14.41 5.25 14.75 5.59 14.75 6C14.75 6.41 14.41 6.75 14 6.75H12.75V17.25H14C14.41 17.25 14.75 17.59 14.75 18C14.75 18.41 14.41 18.75 14 18.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2 9V6.5C2 4.01 4.01 2 6.5 2H9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15 2H17.5C19.99 2 22 4.01 22 6.5V9" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M22 16V17.5C22 19.99 19.99 22 17.5 22H16" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9 22H6.5C4.01 22 2 19.99 2 17.5V15" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<g opacity="0.54">
<path d="M18 12V10M6 12H12H18H6ZM6 12V10V12ZM6 12V14V12ZM18 12V14V12Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 6H14M12 18V6V18ZM12 18H14H12ZM12 18H10H12ZM12 6H10H12Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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