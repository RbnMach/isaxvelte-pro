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
<path d="M19.54 6.53998L16.47 3.46997C15.53 2.52997 14.26 2.01001 12.93 2.01001H8C5 2.01001 3 4.01001 3 7.01001V17.01C3 20.01 5 22.01 8 22.01H16C19 22.01 21 20.01 21 17.01V10.08C21 8.74002 20.47 7.46998 19.54 6.53998Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9.5 14L7.5 16L9.5 18" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M14.5 14L16.5 16L14.5 18" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M19.54 6.54L16.47 3.47C15.53 2.53 14.26 2 12.93 2H8C5 2 3 4 3 7V17C3 20 5 22 8 22H16C19 22 21 20 21 17V10.07C21 8.74 20.47 7.47 19.54 6.54ZM10.03 17.47C10.32 17.76 10.32 18.24 10.03 18.53C9.88 18.68 9.69 18.75 9.5 18.75C9.31 18.75 9.12 18.68 8.97 18.53L6.97 16.53C6.68 16.24 6.68 15.76 6.97 15.47L8.97 13.47C9.26 13.18 9.74 13.18 10.03 13.47C10.32 13.76 10.32 14.24 10.03 14.53L8.56 16L10.03 17.47ZM17.03 16.53L15.03 18.53C14.88 18.68 14.69 18.75 14.5 18.75C14.31 18.75 14.12 18.68 13.97 18.53C13.68 18.24 13.68 17.76 13.97 17.47L15.44 16L13.97 14.53C13.68 14.24 13.68 13.76 13.97 13.47C14.26 13.18 14.74 13.18 15.03 13.47L17.03 15.47C17.32 15.76 17.32 16.24 17.03 16.53Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M3 11V17C3 20 5 22 8 22H16C19 22 21 20 21 17V10.07C21 8.74001 20.47 7.47003 19.54 6.53003L16.47 3.46002C15.53 2.52002 14.26 2 12.93 2H8C5 2 3 4 3 7" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9.5 14L7.5 16L9.5 18" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M14.5 14L16.5 16L14.5 18" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M19.54 6.54001L16.47 3.47C15.53 2.53 14.26 2.01001 12.93 2.01001H8C5 2.01001 3 4.01001 3 7.01001V17.01C3 20.01 5 22.01 8 22.01H16C19 22.01 21 20.01 21 17.01V10.08C21 8.73999 20.47 7.47001 19.54 6.54001Z" fill="{color}"/>
<path d="M9.49945 18.7499C9.30945 18.7499 9.11945 18.6799 8.96945 18.5299L6.96945 16.5299C6.67945 16.2399 6.67945 15.7599 6.96945 15.4699L8.96945 13.4699C9.25945 13.1799 9.73945 13.1799 10.0295 13.4699C10.3195 13.7599 10.3195 14.2399 10.0295 14.5299L8.55945 15.9999L10.0295 17.4699C10.3195 17.7599 10.3195 18.2399 10.0295 18.5299C9.87945 18.6799 9.68945 18.7499 9.49945 18.7499Z" fill="{color}"/>
<path d="M14.4995 18.7499C14.3095 18.7499 14.1195 18.6799 13.9695 18.5299C13.6795 18.2399 13.6795 17.7599 13.9695 17.4699L15.4395 15.9999L13.9695 14.5299C13.6795 14.2399 13.6795 13.7599 13.9695 13.4699C14.2595 13.1799 14.7395 13.1799 15.0295 13.4699L17.0295 15.4699C17.3195 15.7599 17.3195 16.2399 17.0295 16.5299L15.0295 18.5299C14.8795 18.6799 14.6895 18.7499 14.4995 18.7499Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16 22.75H8C4.56 22.75 2.25 20.44 2.25 17V7C2.25 3.56 4.56 1.25 8 1.25H12.93C14.47 1.25 15.91 1.84999 17 2.92999L20.07 6C21.16 7.08 21.75 8.53001 21.75 10.07V17C21.75 20.44 19.44 22.75 16 22.75ZM8 2.75C5.42 2.75 3.75 4.42 3.75 7V17C3.75 19.58 5.42 21.25 8 21.25H16C18.58 21.25 20.25 19.58 20.25 17V10.07C20.25 8.93001 19.81 7.87001 19 7.07001L15.93 4C15.13 3.2 14.06 2.76001 12.92 2.76001H8V2.75Z" fill="{color}"/>
<path d="M9.49945 18.75C9.30945 18.75 9.11945 18.68 8.96945 18.53L6.96945 16.53C6.67945 16.24 6.67945 15.7599 6.96945 15.4699L8.96945 13.4699C9.25945 13.1799 9.73945 13.1799 10.0295 13.4699C10.3195 13.7599 10.3195 14.24 10.0295 14.53L8.55945 16L10.0295 17.4699C10.3195 17.7599 10.3195 18.24 10.0295 18.53C9.87945 18.68 9.68945 18.75 9.49945 18.75Z" fill="{color}"/>
<path d="M14.4995 18.75C14.3095 18.75 14.1195 18.68 13.9695 18.53C13.6795 18.24 13.6795 17.7599 13.9695 17.4699L15.4395 16L13.9695 14.53C13.6795 14.24 13.6795 13.7599 13.9695 13.4699C14.2595 13.1799 14.7395 13.1799 15.0295 13.4699L17.0295 15.4699C17.3195 15.7599 17.3195 16.24 17.0295 16.53L15.0295 18.53C14.8795 18.68 14.6895 18.75 14.4995 18.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M19.54 6.53973L16.47 3.46973C15.53 2.52973 14.26 2.00977 12.93 2.00977H8C5 2.00977 3 4.00977 3 7.00977V17.0098C3 20.0098 5 22.0098 8 22.0098H16C19 22.0098 21 20.0098 21 17.0098V10.0798C21 8.73977 20.47 7.46973 19.54 6.53973Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<g opacity="0.4">
<path d="M9.5 14L7.5 16L9.5 18" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M14.5 14L16.5 16L14.5 18" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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