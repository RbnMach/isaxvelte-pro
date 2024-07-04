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
<path d="M5 15V8" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5.25 22C7.04493 22 8.5 20.5449 8.5 18.75C8.5 16.9551 7.04493 15.5 5.25 15.5C3.45507 15.5 2 16.9551 2 18.75C2 20.5449 3.45507 22 5.25 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5 8C6.65685 8 8 6.65685 8 5C8 3.34315 6.65685 2 5 2C3.34315 2 2 3.34315 2 5C2 6.65685 3.34315 8 5 8Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M19 8C20.6569 8 22 6.65685 22 5C22 3.34315 20.6569 2 19 2C17.3431 2 16 3.34315 16 5C16 6.65685 17.3431 8 19 8Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5.13 15C5.58 13.25 7.18 11.95 9.07 11.96L12.5 11.97C15.12 11.98 17.35 10.3 18.17 7.95996" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <path d="M8.5,18.75c0-1.79-1.46-3.25-3.25-3.25s-3.25,1.46-3.25,3.25,1.46,3.25,3.25,3.25,3.25-1.46,3.25-3.25Z" fill="{color}" stroke-width="0"/>
  <path d="M8,5c0-1.66-1.34-3-3-3s-3,1.34-3,3,1.34,3,3,3,3-1.34,3-3Z" fill="{color}" stroke-width="0"/>
  <path d="M22,5c0-1.66-1.34-3-3-3s-3,1.34-3,3,1.34,3,3,3,3-1.34,3-3Z" fill="{color}" stroke-width="0"/>
  <path d="M18.7,7.04c-.08-.02-.17-.04-.25-.04-.32,0-.61.2-.73.51-.75,2.17-2.8,3.62-5.09,3.62h-3.55s-.01-.01-.02-.01c-1.25,0-2.4.48-3.28,1.26v-6.62c0-.42-.35-.76-.77-.76s-.76.34-.76.76v11.24c0,.42.34.76.76.76s.77-.34.77-.76v-1.85c.41-1.48,1.77-2.51,3.29-2.49h3.53s.02.01.03.01c2.95,0,5.57-1.87,6.54-4.65.14-.4-.07-.84-.47-.98Z" fill="{color}" stroke-width="0"/>
</svg>
	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5 15V8" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5.25 22C7.04493 22 8.5 20.5449 8.5 18.75C8.5 16.9551 7.04493 15.5 5.25 15.5C3.45507 15.5 2 16.9551 2 18.75C2 20.5449 3.45507 22 5.25 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5 8C6.65685 8 8 6.65685 8 5C8 3.34315 6.65685 2 5 2C3.34315 2 2 3.34315 2 5C2 6.65685 3.34315 8 5 8Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M19 8C20.6569 8 22 6.65685 22 5C22 3.34315 20.6569 2 19 2C17.3431 2 16 3.34315 16 5C16 6.65685 17.3431 8 19 8Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5.13086 15C5.58086 13.25 7.18086 11.95 9.07086 11.96L12.5009 11.97C13.3509 11.97 14.1709 11.8 14.9009 11.48" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <path d="M8.5,18.75c0-1.79-1.46-3.25-3.25-3.25s-3.25,1.46-3.25,3.25,1.46,3.25,3.25,3.25,3.25-1.46,3.25-3.25Z" fill="{color}" stroke-width="0"/>
  <path d="M8,5c0-1.66-1.34-3-3-3s-3,1.34-3,3,1.34,3,3,3,3-1.34,3-3Z" fill="{color}" stroke-width="0"/>
  <path d="M22,5c0-1.66-1.34-3-3-3s-3,1.34-3,3,1.34,3,3,3,3-1.34,3-3Z" fill="{color}" stroke-width="0"/>
  <path d="M18.69,7.06c-.08-.03-.17-.04-.25-.04-.31,0-.61.19-.72.51-.75,2.17-2.8,3.62-5.09,3.62h-3.55s-.01,0-.02,0c-1.25,0-2.4.48-3.28,1.26v-6.62c0-.42-.34-.76-.76-.76s-.76.34-.76.76v11.22c0,.42.34.76.76.76s.76-.34.76-.76v-1.85c.41-1.48,1.77-2.51,3.29-2.49h3.53s.02.01.03.01c2.95,0,5.57-1.87,6.54-4.65.14-.4-.07-.84-.48-.96Z" fill="{color}" isolation="isolate" opacity=".4" stroke-width="0"/>
</svg>
	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5 15.75C4.59 15.75 4.25 15.41 4.25 15V8C4.25 7.59 4.59 7.25 5 7.25C5.41 7.25 5.75 7.59 5.75 8V15C5.75 15.41 5.41 15.75 5 15.75Z" fill="{color}"/>
<path d="M5.25 22.75C3.04 22.75 1.25 20.96 1.25 18.75C1.25 16.54 3.04 14.75 5.25 14.75C7.46 14.75 9.25 16.54 9.25 18.75C9.25 20.96 7.46 22.75 5.25 22.75ZM5.25 16.25C3.87 16.25 2.75 17.37 2.75 18.75C2.75 20.13 3.87 21.25 5.25 21.25C6.63 21.25 7.75 20.13 7.75 18.75C7.75 17.37 6.63 16.25 5.25 16.25Z" fill="{color}"/>
<path d="M5 8.75C2.93 8.75 1.25 7.07 1.25 5C1.25 2.93 2.93 1.25 5 1.25C7.07 1.25 8.75 2.93 8.75 5C8.75 7.07 7.07 8.75 5 8.75ZM5 2.75C3.76 2.75 2.75 3.76 2.75 5C2.75 6.24 3.76 7.25 5 7.25C6.24 7.25 7.25 6.24 7.25 5C7.25 3.76 6.24 2.75 5 2.75Z" fill="{color}"/>
<path d="M19 8.75C16.93 8.75 15.25 7.07 15.25 5C15.25 2.93 16.93 1.25 19 1.25C21.07 1.25 22.75 2.93 22.75 5C22.75 7.07 21.07 8.75 19 8.75ZM19 2.75C17.76 2.75 16.75 3.76 16.75 5C16.75 6.24 17.76 7.25 19 7.25C20.24 7.25 21.25 6.24 21.25 5C21.25 3.76 20.24 2.75 19 2.75Z" fill="{color}"/>
<path d="M5.12962 15.7503C5.06962 15.7503 5.00962 15.7403 4.93962 15.7303C4.53962 15.6303 4.29962 15.2203 4.39962 14.8203C4.94962 12.7003 6.85962 11.2203 9.04962 11.2203C9.05962 11.2203 9.05962 11.2203 9.06962 11.2203L12.4996 11.2303C12.5096 11.2303 12.5096 11.2303 12.5196 11.2303C14.7396 11.2303 16.7296 9.82026 17.4596 7.72026C17.5996 7.33026 18.0196 7.12027 18.4096 7.26027C18.7996 7.40027 19.0096 7.82025 18.8696 8.21025C17.9296 10.9202 15.3396 12.7003 12.4896 12.7303L9.05962 12.7203H9.04962C7.53962 12.7203 6.22962 13.7403 5.84962 15.2003C5.76962 15.5303 5.45962 15.7503 5.12962 15.7503Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5.25 22C7.04493 22 8.5 20.5449 8.5 18.75C8.5 16.9551 7.04493 15.5 5.25 15.5C3.45507 15.5 2 16.9551 2 18.75C2 20.5449 3.45507 22 5.25 22Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5 8C6.65685 8 8 6.65685 8 5C8 3.34315 6.65685 2 5 2C3.34315 2 2 3.34315 2 5C2 6.65685 3.34315 8 5 8Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M19 8C20.6569 8 22 6.65685 22 5C22 3.34315 20.6569 2 19 2C17.3431 2 16 3.34315 16 5C16 6.65685 17.3431 8 19 8Z" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<g opacity="0.4">
<path d="M5 15V8" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5.12891 15C5.57891 13.25 7.1789 11.95 9.0689 11.96L12.4989 11.97C15.1189 11.98 17.3489 10.3 18.1689 7.95996" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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