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
<path d="M17 20H7C4 20 2 18 2 15V9C2 6 4 4 7 4H17C20 4 22 6 22 9V15C22 18 20 20 17 20Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.4001 9.50006L13.9001 11.0001C14.8001 11.6001 14.8001 12.5001 13.9001 13.1001L11.4001 14.6001C10.4001 15.2001 9.6001 14.7001 9.6001 13.6001V10.6001C9.6001 9.30006 10.4001 8.90006 11.4001 9.50006Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M17 4H7C4 4 2 6 2 9V15C2 18 4 20 7 20H17C20 20 22 18 22 15V9C22 6 20 4 17 4ZM13.89 13.03L11.42 14.51C10.42 15.11 9.59998 14.65 9.59998 13.48V10.51C9.59998 9.34001 10.42 8.88001 11.42 9.48001L13.89 10.96C14.84 11.54 14.84 12.46 13.89 13.03Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2 9C2 6 4 4 7 4H17C20 4 22 6 22 9V15C22 18 20 20 17 20H7C4 20 2 18 2 15V13.59" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.4196 9.49009L13.8896 10.9701C14.8296 11.5401 14.8296 12.4601 13.8896 13.0301L11.4196 14.5101C10.4196 15.1101 9.59961 14.6501 9.59961 13.4801V10.5101C9.59961 9.35011 10.4196 8.89009 11.4196 9.49009Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M22.667 26.667h-13.333c-4 0-6.667-2.667-6.667-6.667v-8c0-4 2.667-6.667 6.667-6.667h13.333c4 0 6.667 2.667 6.667 6.667v8c0 4-2.667 6.667-6.667 6.667z"></path>
<path fill="{color}" d="M15.226 12.653l3.293 1.973c1.253 0.76 1.253 1.987 0 2.747l-3.293 1.973c-1.333 0.8-2.427 0.187-2.427-1.373v-3.96c0-1.547 1.093-2.16 2.427-1.36z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M17 20.75H7C3.56 20.75 1.25 18.44 1.25 15V9C1.25 5.56 3.56 3.25 7 3.25H17C20.44 3.25 22.75 5.56 22.75 9V15C22.75 18.44 20.44 20.75 17 20.75ZM7 4.75C4.42 4.75 2.75 6.42 2.75 9V15C2.75 17.58 4.42 19.25 7 19.25H17C19.58 19.25 21.25 17.58 21.25 15V9C21.25 6.42 19.58 4.75 17 4.75H7Z" fill="{color}"/>
<path d="M10.5897 15.5302C10.2997 15.5302 10.0197 15.4602 9.76965 15.3202C9.18965 14.9902 8.84961 14.3202 8.84961 13.4902V10.5302C8.84961 9.70022 9.17965 9.03023 9.76965 8.70023C10.3497 8.37023 11.0996 8.4302 11.8096 8.8602L14.2797 10.3402C14.9597 10.7502 15.3496 11.3602 15.3496 12.0102C15.3496 12.6602 14.9597 13.2702 14.2797 13.6802L11.8096 15.1602C11.3996 15.4002 10.9797 15.5302 10.5897 15.5302ZM10.5897 9.97022C10.5497 9.97022 10.5196 9.98021 10.4996 9.99021C10.4296 10.0302 10.3496 10.2102 10.3496 10.5202V13.4802C10.3496 13.7802 10.4296 13.9602 10.4996 14.0102C10.5796 14.0502 10.7697 14.0302 11.0297 13.8702L13.4996 12.3902C13.7496 12.2402 13.8397 12.0902 13.8397 12.0002C13.8397 11.9102 13.7496 11.7702 13.4996 11.6102L11.0297 10.1302C10.8497 10.0202 10.6897 9.97022 10.5897 9.97022Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M17 20H7C4 20 2 18 2 15V9C2 6 4 4 7 4H17C20 4 22 6 22 9V15C22 18 20 20 17 20Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M11.4196 9.49009L13.8896 10.9701C14.8296 11.5401 14.8296 12.4601 13.8896 13.0301L11.4196 14.5101C10.4196 15.1101 9.59961 14.6501 9.59961 13.4801V10.5101C9.59961 9.35011 10.4196 8.89009 11.4196 9.49009Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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