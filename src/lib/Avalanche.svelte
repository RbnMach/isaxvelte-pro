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
<path d="M6.10004 15.5999L11.7 5.9999C11.9 5.6999 12.3 5.6999 12.5 5.9999L14 7.9999C14.4 8.5999 14.5 9.3999 14.1 9.9999L10.8 15.2999C10.5 15.7999 9.90004 16.1999 9.30004 16.1999H6.40004C6.10004 16.2999 5.90004 15.8999 6.10004 15.5999Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.2001 12.3998L13.3001 15.5998C13.1001 15.8998 13.3001 16.2998 13.7001 16.2998H17.5001C17.9001 16.2998 18.1001 15.8998 17.9001 15.5998L16.0001 12.3998C15.8001 12.0998 15.4001 12.0998 15.2001 12.3998Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM10.72 15.41C10.39 15.94 9.80999 16.26 9.17999 16.26H6.44C6.09 16.26 5.86999 15.88 6.04999 15.58L11.66 5.97C11.82 5.69 12.22 5.67 12.41 5.93L13.97 8.02C14.42 8.62 14.45 9.43 14.06 10.07L10.72 15.41ZM17.55 16.26H13.71C13.36 16.26 13.14 15.88 13.32 15.57L15.24 12.37C15.42 12.08 15.84 12.08 16.02 12.37L17.94 15.57C18.12 15.87 17.9 16.26 17.55 16.26Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M6.06033 15.58L11.6703 5.96995C11.8303 5.68995 12.2303 5.66995 12.4203 5.92995L13.9803 8.01995C14.4303 8.61995 14.4603 9.42995 14.0703 10.0699L10.7303 15.4199C10.4003 15.9499 9.82034 16.2699 9.19034 16.2699H6.45035C6.10035 16.2599 5.88033 15.88 6.06033 15.58Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.2401 12.3701L13.3201 15.5701C13.1401 15.8701 13.3601 16.2601 13.7101 16.2601H17.5501C17.9001 16.2601 18.1201 15.8801 17.9401 15.5701L16.0201 12.3701C15.8501 12.0801 15.4201 12.0801 15.2401 12.3701Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.19997 2.3 7.96997 2.85" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" d="M8.080 20.774l7.48-12.813c0.213-0.373 0.747-0.4 1-0.053l2.080 2.787c0.6 0.8 0.64 1.88 0.12 2.733l-4.453 7.133c-0.44 0.707-1.213 1.133-2.053 1.133h-3.653c-0.467-0.013-0.76-0.52-0.52-0.92z"></path>
<path fill="{color}" d="M20.32 16.494l-2.56 4.267c-0.24 0.4 0.053 0.92 0.52 0.92h5.12c0.467 0 0.76-0.507 0.52-0.92l-2.56-4.267c-0.227-0.387-0.8-0.387-1.040 0z"></path>
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M9.19046 17.0099H6.45047C6.02047 17.0099 5.62043 16.7799 5.41043 16.4099C5.20043 16.0399 5.20043 15.5799 5.41043 15.1999L11.0105 5.58991C11.2105 5.23991 11.5804 5.01991 11.9804 4.98991C12.3804 4.95991 12.7705 5.14992 13.0105 5.46992L14.5805 7.55991C15.2105 8.39991 15.2605 9.55991 14.7005 10.4599L11.3604 15.8099C10.8904 16.5599 10.0805 17.0099 9.19046 17.0099ZM6.96048 15.5099H9.18045C9.55045 15.5099 9.89047 15.3199 10.0805 15.0099L13.4204 9.65992C13.6504 9.28992 13.6305 8.80991 13.3705 8.45991L12.0705 6.72992L6.96048 15.5099Z" fill="{color}"/>
<path d="M17.5502 17.0099H13.7102C13.2802 17.0099 12.8802 16.7799 12.6602 16.3999C12.4502 16.0199 12.4502 15.5599 12.6702 15.1899L14.5902 11.9899C15.0302 11.2599 16.2102 11.2599 16.6502 11.9899L18.5702 15.1899C18.7902 15.5599 18.8002 16.0299 18.5802 16.3999C18.3902 16.7699 17.9802 17.0099 17.5502 17.0099ZM14.2402 15.5099H17.0302L15.6302 13.1799L14.2402 15.5099Z" fill="{color}"/>
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M6.06033 15.5802L11.6703 5.9702C11.8303 5.6902 12.2303 5.67019 12.4203 5.93019L13.9803 8.02019C14.4303 8.62019 14.4603 9.43019 14.0703 10.0702L10.7303 15.4202C10.4003 15.9502 9.82034 16.2702 9.19034 16.2702H6.45035C6.10035 16.2602 5.88033 15.8802 6.06033 15.5802Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M15.2401 12.3698L13.3201 15.5698C13.1401 15.8698 13.3601 16.2598 13.7101 16.2598H17.5501C17.9001 16.2598 18.1201 15.8798 17.9401 15.5698L16.0201 12.3698C15.8501 12.0798 15.4201 12.0798 15.2401 12.3698Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
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