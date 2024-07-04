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
<path d="M16.44 8.8999C20.04 9.2099 21.51 11.0599 21.51 15.1099V15.2399C21.51 19.7099 19.72 21.4999 15.25 21.4999H8.73998C4.26998 21.4999 2.47998 19.7099 2.47998 15.2399V15.1099C2.47998 11.0899 3.92998 9.2399 7.46998 8.9099" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 15.0001V3.62012" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.35 5.85L12 2.5L8.65002 5.85" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.8 9H12.75V15.25C12.75 15.66 12.41 16 12 16C11.59 16 11.25 15.66 11.25 15.25V9H7.2C4 9 2 11 2 14.2V16.79C2 20 4 22 7.2 22H16.79C19.99 22 21.99 20 21.99 16.8V14.2C22 11 20 9 16.8 9Z" fill="{color}"/>
<path d="M12.7498 4.56141L14.8198 6.63141C14.9698 6.78141 15.1598 6.85141 15.3498 6.85141C15.5398 6.85141 15.7298 6.78141 15.8798 6.63141C16.1698 6.34141 16.1698 5.86141 15.8798 5.57141L12.5298 2.22141C12.2398 1.93141 11.7598 1.93141 11.4698 2.22141L8.11984 5.57141C7.82984 5.86141 7.82984 6.34141 8.11984 6.63141C8.40984 6.92141 8.88984 6.92141 9.17984 6.63141L11.2498 4.56141V9.00141H12.7498V4.56141Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 15.0001V3.62012" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.3504 5.85L12.0004 2.5L8.65039 5.85" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.74047 21.4999C4.27047 21.4999 2.48047 19.7099 2.48047 15.2399V15.1099C2.48047 11.0899 3.93047 9.23991 7.47047 8.90991" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16.4398 8.8999C20.0398 9.2099 21.5098 11.0599 21.5098 15.1099V15.2399C21.5098 19.7099 19.7198 21.4999 15.2498 21.4999H13.0098" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M16.8 9H7.2C4 9 2 11 2 14.2V16.79C2 20 4 22 7.2 22H16.79C19.99 22 21.99 20 21.99 16.8V14.2C22 11 20 9 16.8 9Z" fill="{color}"/>
<path d="M15.8798 5.56994L12.5298 2.21994C12.2398 1.92994 11.7598 1.92994 11.4698 2.21994L8.11984 5.56994C7.82984 5.85994 7.82984 6.33994 8.11984 6.62994C8.40984 6.91994 8.88984 6.91994 9.17984 6.62994L11.2498 4.55994V15.2499C11.2498 15.6599 11.5898 15.9999 11.9998 15.9999C12.4098 15.9999 12.7498 15.6599 12.7498 15.2499V4.55994L14.8198 6.62994C14.9698 6.77994 15.1598 6.84994 15.3498 6.84994C15.5398 6.84994 15.7298 6.77994 15.8798 6.62994C16.1798 6.33994 16.1798 5.86994 15.8798 5.56994Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15.2605 22.25H8.74047C3.83047 22.25 1.73047 20.15 1.73047 15.24V15.11C1.73047 10.67 3.48047 8.53003 7.40047 8.16003C7.80047 8.13003 8.18047 8.43003 8.22047 8.84003C8.26047 9.25003 7.96047 9.62003 7.54047 9.66003C4.40047 9.95003 3.23047 11.43 3.23047 15.12V15.25C3.23047 19.32 4.67047 20.76 8.74047 20.76H15.2605C19.3305 20.76 20.7705 19.32 20.7705 15.25V15.12C20.7705 11.41 19.5805 9.93003 16.3805 9.66003C15.9705 9.62003 15.6605 9.26003 15.7005 8.85003C15.7405 8.44003 16.0905 8.13003 16.5105 8.17003C20.4905 8.51003 22.2705 10.66 22.2705 15.13V15.26C22.2705 20.15 20.1705 22.25 15.2605 22.25Z" fill="{color}"/>
<path d="M12 15.7501C11.59 15.7501 11.25 15.4101 11.25 15.0001V3.62012C11.25 3.21012 11.59 2.87012 12 2.87012C12.41 2.87012 12.75 3.21012 12.75 3.62012V15.0001C12.75 15.4101 12.41 15.7501 12 15.7501Z" fill="{color}"/>
<path d="M15.3498 6.59994C15.1598 6.59994 14.9698 6.52994 14.8198 6.37994L11.9998 3.55994L9.17984 6.37994C8.88984 6.66994 8.40984 6.66994 8.11984 6.37994C7.82984 6.08994 7.82984 5.60994 8.11984 5.31994L11.4698 1.96994C11.7598 1.67994 12.2398 1.67994 12.5298 1.96994L15.8798 5.31994C16.1698 5.60994 16.1698 6.08994 15.8798 6.37994C15.7398 6.52994 15.5398 6.59994 15.3498 6.59994Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.4405 8.8999C20.0405 9.2099 21.5105 11.0599 21.5105 15.1099V15.2399C21.5105 19.7099 19.7205 21.4999 15.2505 21.4999H8.74047C4.27047 21.4999 2.48047 19.7099 2.48047 15.2399V15.1099C2.48047 11.0899 3.93047 9.2399 7.47047 8.9099" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<g opacity="0.4">
<path d="M12 15.0001V3.62012" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.3504 5.85L12.0004 2.5L8.65039 5.85" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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