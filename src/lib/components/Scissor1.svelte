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
<path d="M5.5 10C7.433 10 9 8.433 9 6.5C9 4.567 7.433 3 5.5 3C3.567 3 2 4.567 2 6.5C2 8.433 3.567 10 5.5 10Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5.5 21C7.433 21 9 19.433 9 17.5C9 15.567 7.433 14 5.5 14C3.567 14 2 15.567 2 17.5C2 19.433 3.567 21 5.5 21Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M22 6L8.64999 15.98" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M22 17.97L8.64999 7.97998" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5.5 10C7.433 10 9 8.433 9 6.5C9 4.567 7.433 3 5.5 3C3.567 3 2 4.567 2 6.5C2 8.433 3.567 10 5.5 10Z" fill="{color}"/>
<path d="M5.5 21C7.433 21 9 19.433 9 17.5C9 15.567 7.433 14 5.5 14C3.567 14 2 15.567 2 17.5C2 19.433 3.567 21 5.5 21Z" fill="{color}"/>
<path d="M15.2491 11.9803L22.4491 6.60027C22.7791 6.35027 22.8491 5.88027 22.5991 5.55027C22.3491 5.22027 21.8791 5.15027 21.5491 5.40027L13.9991 11.0503L8.4491 6.89027C8.1191 6.65027 7.6491 6.71027 7.3991 7.04027C7.1491 7.37027 7.2191 7.84027 7.5491 8.09027L12.7491 11.9803L6.8491 16.4003C6.5191 16.6503 6.4491 17.1203 6.6991 17.4503C6.8491 17.6503 7.0691 17.7503 7.2991 17.7503C7.4591 17.7503 7.6091 17.7003 7.7491 17.6003L13.9991 12.9203L21.5491 18.5703C21.6791 18.6703 21.8391 18.7203 21.9991 18.7203C22.2291 18.7203 22.4491 18.6203 22.5991 18.4203C22.8491 18.0903 22.7791 17.6203 22.4491 17.3703L15.2491 11.9803Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5.5 3C7.43 3 9 4.57 9 6.5C9 8.43 7.43 10 5.5 10C3.57 10 2 8.43 2 6.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5.5 21C7.433 21 9 19.433 9 17.5C9 15.567 7.433 14 5.5 14C3.567 14 2 15.567 2 17.5C2 19.433 3.567 21 5.5 21Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M22.0004 6L8.65039 15.98" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M22.0004 17.97L8.65039 7.97998" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5.5 10C7.433 10 9 8.433 9 6.5C9 4.567 7.433 3 5.5 3C3.567 3 2 4.567 2 6.5C2 8.433 3.567 10 5.5 10Z" fill="{color}"/>
<path d="M5.5 21C7.433 21 9 19.433 9 17.5C9 15.567 7.433 14 5.5 14C3.567 14 2 15.567 2 17.5C2 19.433 3.567 21 5.5 21Z" fill="{color}"/>
<path opacity="0.4" d="M15.2491 11.9798L22.4491 6.59978C22.7791 6.34978 22.8491 5.87978 22.5991 5.54978C22.3491 5.21978 21.8791 5.14978 21.5491 5.39978L13.9991 11.0498L8.4491 6.89978C8.1191 6.64978 7.64908 6.71978 7.39908 7.04978C7.14908 7.37978 7.21908 7.84978 7.54908 8.09978L12.7491 11.9898L6.8491 16.4098C6.5191 16.6598 6.4491 17.1298 6.6991 17.4598C6.8491 17.6598 7.06908 17.7598 7.29908 17.7598C7.45908 17.7598 7.60909 17.7098 7.74909 17.6098L14.0091 12.9298L21.5591 18.5798C21.6891 18.6798 21.8491 18.7298 22.0091 18.7298C22.2391 18.7298 22.4591 18.6298 22.6091 18.4298C22.8591 18.0998 22.7891 17.6298 22.4591 17.3798L15.2491 11.9798Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5.5 10.75C3.16 10.75 1.25 8.84 1.25 6.5C1.25 4.16 3.16 2.25 5.5 2.25C7.84 2.25 9.75 4.16 9.75 6.5C9.75 8.84 7.84 10.75 5.5 10.75ZM5.5 3.75C3.98 3.75 2.75 4.98 2.75 6.5C2.75 8.02 3.98 9.25 5.5 9.25C7.02 9.25 8.25 8.02 8.25 6.5C8.25 4.98 7.02 3.75 5.5 3.75Z" fill="{color}"/>
<path d="M5.5 21.75C3.16 21.75 1.25 19.84 1.25 17.5C1.25 15.16 3.16 13.25 5.5 13.25C7.84 13.25 9.75 15.16 9.75 17.5C9.75 19.84 7.84 21.75 5.5 21.75ZM5.5 14.75C3.98 14.75 2.75 15.98 2.75 17.5C2.75 19.02 3.98 20.25 5.5 20.25C7.02 20.25 8.25 19.02 8.25 17.5C8.25 15.98 7.02 14.75 5.5 14.75Z" fill="{color}"/>
<path d="M8.65066 16.7303C8.42066 16.7303 8.20065 16.6303 8.05065 16.4303C7.80065 16.1003 7.87068 15.6303 8.20068 15.3803L21.5507 5.40027C21.8807 5.15027 22.3507 5.22027 22.6007 5.55027C22.8507 5.88027 22.7807 6.35027 22.4507 6.60027L9.10067 16.5803C8.97067 16.6803 8.81066 16.7303 8.65066 16.7303Z" fill="{color}"/>
<path d="M22.0007 18.72C21.8407 18.72 21.6907 18.67 21.5507 18.57L8.20068 8.59002C7.87068 8.34002 7.80065 7.87002 8.05065 7.54002C8.30065 7.21002 8.77067 7.14002 9.10067 7.39002L22.4507 17.37C22.7807 17.62 22.8507 18.09 22.6007 18.42C22.4507 18.61 22.2307 18.72 22.0007 18.72Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5.5 10C7.433 10 9 8.433 9 6.5C9 4.567 7.433 3 5.5 3C3.567 3 2 4.567 2 6.5C2 8.433 3.567 10 5.5 10Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5.5 21C7.433 21 9 19.433 9 17.5C9 15.567 7.433 14 5.5 14C3.567 14 2 15.567 2 17.5C2 19.433 3.567 21 5.5 21Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<g opacity="0.4">
<path d="M22.0004 6L8.65039 15.98" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M22.0004 17.97L8.65039 7.97998" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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