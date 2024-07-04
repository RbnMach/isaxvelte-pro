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
<path d="M17.9 19.7001C16.2 21.2001 13.9 22.1001 11.4 22.0001C6.19995 21.9001 2.19995 17.4001 2.19995 12.2001V5.2001C2.19995 4.8001 2.69995 4.5001 3.09995 4.8001L17.9 19.7001Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6.19995 4.29998C7.89995 2.79998 10.2 1.89998 12.6 1.99998C17.7 2.09998 21.7 6.49998 21.7 11.7V18.7C21.7 19.1 21.2 19.4 20.8 19.1L6.19995 4.29998Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M17.9007 19.6786C16.1807 21.1786 13.9107 22.0686 11.4207 21.9986C6.25072 21.8586 2.2207 17.4086 2.2207 12.2386V5.20857C2.2207 4.75857 2.76071 4.53856 3.07071 4.85856L17.9007 19.6786Z" fill="{color}"/>
<path d="M6.2207 4.29998C7.9307 2.80998 10.1807 1.92998 12.6507 1.99998C17.7807 2.13998 21.7707 6.54997 21.7707 11.68V18.64C21.7707 19.09 21.2307 19.31 20.9207 18.99L6.2207 4.29998Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2.2207 6.98001V5.20001C2.2207 4.75001 2.76071 4.53002 3.07071 4.85002L17.9007 19.68C16.1807 21.18 13.9107 22.07 11.4207 22C6.25072 21.86 2.2207 17.41 2.2207 12.24V11.08" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6.2207 4.29998C7.9307 2.80998 10.1807 1.92998 12.6507 1.99998C17.7807 2.13998 21.7707 6.54997 21.7707 11.68V18.64C21.7707 19.09 21.2307 19.31 20.9207 18.99L6.2207 4.29998Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M23.868 26.24c-2.293 2-5.32 3.187-8.64 3.093-6.893-0.187-12.267-6.12-12.267-13.013v-9.373c0-0.6 0.72-0.893 1.133-0.467l19.773 19.76z"></path>
<path fill="{color}" d="M8.294 5.733c2.28-1.987 5.28-3.16 8.573-3.067 6.84 0.187 12.16 6.067 12.16 12.907v9.28c0 0.6-0.72 0.893-1.133 0.467l-19.6-19.587z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11.7005 22.7498C11.6005 22.7498 11.5105 22.7498 11.4105 22.7498C5.93046 22.5998 1.48047 17.8798 1.48047 12.2398V5.20978C1.48047 4.69978 1.78046 4.24978 2.25046 4.05978C2.72046 3.86978 3.25044 3.96978 3.61044 4.32978L18.4405 19.1598C18.5905 19.3098 18.6705 19.5098 18.6605 19.7198C18.6505 19.9298 18.5605 20.1198 18.4005 20.2598C16.5405 21.8698 14.1705 22.7498 11.7005 22.7498ZM2.98047 5.80978V12.2398C2.98047 17.0798 6.78047 21.1198 11.4505 21.2498C13.3805 21.2898 15.2505 20.7298 16.7805 19.6198L2.98047 5.80978Z" fill="{color}"/>
<path d="M21.2696 19.9001C20.9496 19.9001 20.6296 19.7701 20.3896 19.5301L5.68959 4.83008C5.53959 4.68008 5.45959 4.48008 5.46959 4.27008C5.47959 4.06008 5.5696 3.87007 5.7296 3.73007C7.6396 2.06007 10.1096 1.17008 12.6696 1.25008C18.0996 1.40008 22.5196 6.08007 22.5196 11.6801V18.6401C22.5196 19.1501 22.2196 19.6001 21.7496 19.7901C21.5996 19.8601 21.4396 19.9001 21.2696 19.9001ZM7.34959 4.37007L21.0296 18.0501V11.6901C21.0296 6.90008 17.2596 2.89007 12.6296 2.76007C10.7196 2.72007 8.86959 3.27007 7.34959 4.37007Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M17.8997 19.68C16.1797 21.18 13.9097 22.07 11.4197 22C6.24974 21.86 2.21973 17.41 2.21973 12.24V5.21004C2.21973 4.76004 2.75973 4.54003 3.06973 4.86003L17.8997 19.68Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6.21973 4.29998C7.92973 2.80998 10.1797 1.92998 12.6497 1.99998C17.7797 2.13998 21.7697 6.54997 21.7697 11.68V18.64C21.7697 19.09 21.2297 19.31 20.9197 18.99L6.21973 4.29998Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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