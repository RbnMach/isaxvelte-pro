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
<path d="M3 8.2V15.8C3 16.5 3.4 17.2 4 17.5L11 21.4C11.6 21.7 12.3 21.7 12.9 21.4L19.9 17.5C20.5 17.1 20.9 16.5 20.9 15.8V8.2C20.9 7.5 20.5 6.8 19.9 6.5L12.9 2.6C12.3 2.3 11.6 2.3 11 2.6L4 6.4C3.4 6.8 3 7.5 3 8.2Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M3 8.18141V15.8314C3 16.4814 3.46 17.2614 4.03 17.5814L11.03 21.4714C11.56 21.7714 12.44 21.7714 12.97 21.4714L19.97 17.5814C20.54 17.2714 21 16.4814 21 15.8314V8.18141C21 7.53141 20.54 6.75141 19.97 6.43141L12.97 2.54141C12.44 2.24141 11.56 2.24141 11.03 2.54141L4.03 6.43141C3.46 6.74141 3 7.53141 3 8.18141Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M3 12.6599V15.8199C3 16.4699 3.46 17.2499 4.03 17.5699L11.03 21.4599C11.56 21.7599 12.44 21.7599 12.97 21.4599L19.97 17.5699C20.54 17.2599 21 16.4699 21 15.8199V8.17994C21 7.52994 20.54 6.74994 19.97 6.42994L12.97 2.53994C12.44 2.23994 11.56 2.23994 11.03 2.53994L4.03 6.42994C3.46 6.73994 3 7.52994 3 8.17994" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" d="M4 10.907v10.2c0 0.867 0.613 1.907 1.373 2.333l9.333 5.187c0.707 0.4 1.88 0.4 2.587 0l9.333-5.187c0.76-0.413 1.373-1.467 1.373-2.333v-10.2c0-0.867-0.613-1.907-1.373-2.333l-9.333-5.187c-0.707-0.4-1.88-0.4-2.587 0l-9.333 5.187c-0.76 0.413-1.373 1.467-1.373 2.333z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22.4302C11.52 22.4302 11.05 22.3202 10.66 22.1102L3.66 18.2202C2.85 17.7702 2.25 16.7402 2.25 15.8202V8.1802C2.25 7.2602 2.86001 6.2202 3.67001 5.7802L10.67 1.8902C11.43 1.4702 12.58 1.4702 13.34 1.8902L20.34 5.7802C21.15 6.2302 21.75 7.2602 21.75 8.1802V15.8302C21.75 16.7502 21.14 17.7902 20.33 18.2302L13.33 22.1202C12.96 22.3302 12.48 22.4302 12 22.4302ZM12 3.0702C11.77 3.0702 11.55 3.1102 11.39 3.2002L4.39001 7.0902C4.06001 7.2702 3.75 7.8002 3.75 8.1802V15.8302C3.75 16.2102 4.06001 16.7402 4.39001 16.9202L11.39 20.8102C11.7 20.9802 12.3 20.9802 12.6 20.8102L19.6 16.9202C19.93 16.7402 20.24 16.2102 20.24 15.8302V8.1802C20.24 7.8002 19.93 7.2702 19.6 7.0902L12.6 3.2002C12.45 3.1102 12.23 3.0702 12 3.0702Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M3 8.17994V15.8299C3 16.4799 3.46 17.2599 4.03 17.5799L11.03 21.4699C11.56 21.7699 12.44 21.7699 12.97 21.4699L19.97 17.5799C20.54 17.2699 21 16.4799 21 15.8299V8.17994C21 7.52994 20.54 6.74994 19.97 6.42994L12.97 2.53994C12.44 2.23994 11.56 2.23994 11.03 2.53994L4.03 6.42994C3.46 6.73994 3 7.52994 3 8.17994Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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