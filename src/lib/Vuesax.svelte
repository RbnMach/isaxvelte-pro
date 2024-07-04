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
<path d="M21 8L12 22L2.95996 8" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3 4H6L12 13L18 4H21L12 18L3 4Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8 3L12 9L16 3L13.2 4V2H10.8V4L8 3Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11.9998 22.7487C11.7498 22.7487 11.5098 22.6187 11.3698 22.4087L2.32981 8.40866C2.10981 8.05866 2.20981 7.59865 2.54981 7.36865C2.89981 7.14865 3.35982 7.23865 3.58982 7.58865L11.9898 20.6086L20.3598 7.58865C20.5798 7.23865 21.0498 7.13864 21.3998 7.35864C21.7498 7.57864 21.8498 8.04865 21.6298 8.39865L12.6298 22.3986C12.4898 22.6186 12.2598 22.7487 11.9998 22.7487Z" fill="{color}"/>
<path d="M3.91975 4H5.73972C5.90972 4 6.05974 4.08 6.15974 4.22L11.5997 12.37C11.7997 12.67 12.2297 12.67 12.4297 12.37L17.8697 4.22C17.9597 4.08 18.1197 4 18.2897 4H20.1097C20.5097 4 20.7397 4.43999 20.5297 4.76999L12.4497 17.35C12.2497 17.66 11.8097 17.66 11.6097 17.35L3.52973 4.76999C3.27973 4.43999 3.51975 4 3.91975 4Z" fill="{color}"/>
<path d="M9.41952 3.5C8.96952 3.34 8.56951 3.85 8.83951 4.25L11.5895 8.38C11.7895 8.68001 12.2195 8.68001 12.4195 8.38L15.1695 4.26001C15.4395 3.86001 15.0395 3.35001 14.5895 3.51001L13.2095 4V2.5C13.2095 2.22 12.9895 2 12.7095 2H11.3095C11.0295 2 10.8095 2.22 10.8095 2.5V4L9.41952 3.5Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M21.0009 8L12.0009 22L2.96094 8" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.53 12.52L12 18L3 4H6L12 13L18 4H21L18.01 8.64999" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8 3L12 9L16 3L13.2 4V2H10.8V4L8 3Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" d="M16 30.333c-0.333 0-0.653-0.173-0.84-0.453l-12.053-18.667c-0.293-0.467-0.16-1.080 0.293-1.387 0.467-0.293 1.080-0.173 1.387 0.293l11.2 17.36 11.16-17.36c0.293-0.467 0.92-0.6 1.387-0.307s0.6 0.92 0.307 1.387l-12 18.667c-0.187 0.293-0.493 0.467-0.84 0.467z"></path>
<path fill="{color}" opacity="0.4" d="M5.226 5.333h2.427c0.227 0 0.427 0.107 0.56 0.293l7.253 10.867c0.267 0.4 0.84 0.4 1.107 0l7.253-10.867c0.12-0.187 0.333-0.293 0.56-0.293h2.427c0.533 0 0.84 0.587 0.56 1.027l-10.773 16.773c-0.267 0.413-0.853 0.413-1.12 0l-10.773-16.773c-0.333-0.44-0.013-1.027 0.52-1.027z"></path>
<path fill="{color}" d="M10.667 4l4.773 7.173c0.267 0.4 0.84 0.4 1.107 0l4.787-7.173-3.733 1.333v-2.667h-3.2v2.667l-3.733-1.333z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M11.9998 22.7501C11.7498 22.7501 11.5098 22.6201 11.3698 22.4101L2.32981 8.41012C2.10981 8.06012 2.20981 7.60011 2.54981 7.37011C2.89981 7.15011 3.35982 7.24011 3.58982 7.59011L11.9898 20.6101L20.3598 7.59011C20.5798 7.24011 21.0498 7.1401 21.3998 7.3601C21.7498 7.5801 21.8498 8.05011 21.6298 8.40011L12.6298 22.4001C12.4898 22.6201 12.2598 22.7501 11.9998 22.7501Z" fill="{color}"/>
<path d="M11.9996 18.7498C11.7396 18.7498 11.5096 18.6198 11.3696 18.4098L2.36956 4.40976C2.21956 4.17976 2.20956 3.88975 2.33956 3.64975C2.46956 3.40975 2.71956 3.25977 2.99956 3.25977H5.99956C6.24956 3.25977 6.47956 3.37975 6.61956 3.58975L11.9996 11.6497L17.3796 3.58975C17.5196 3.37975 17.7496 3.25977 17.9996 3.25977H20.9996C21.2696 3.25977 21.5296 3.40975 21.6596 3.64975C21.7896 3.88975 21.7796 4.17976 21.6296 4.40976L12.6296 18.4098C12.4896 18.6198 12.2596 18.7498 11.9996 18.7498ZM4.36956 4.74976L11.9996 16.6097L19.6296 4.74976H18.3996L12.6196 13.4198C12.3396 13.8398 11.6496 13.8398 11.3696 13.4198L5.58956 4.74976H4.36956Z" fill="{color}"/>
<path d="M11.9998 9.75C11.7498 9.75 11.5198 9.63001 11.3798 9.42001L7.37985 3.42001C7.19985 3.15001 7.20985 2.80001 7.40985 2.54001C7.60985 2.29001 7.94984 2.18999 8.24984 2.29999L10.0498 2.94V2C10.0498 1.59 10.3898 1.25 10.7998 1.25H13.1999C13.6099 1.25 13.9499 1.59 13.9499 2V2.94L15.7498 2.29999C16.0498 2.18999 16.3898 2.29001 16.5898 2.54001C16.7898 2.79001 16.7998 3.15001 16.6198 3.42001L12.6198 9.42001C12.4798 9.62001 12.2498 9.75 11.9998 9.75ZM9.87985 4.47L11.9998 7.64999L14.1198 4.47L13.4499 4.70999C13.2199 4.78999 12.9698 4.76 12.7698 4.62C12.5698 4.48 12.4499 4.25001 12.4499 4.01001V2.76001H11.5498V4C11.5498 4.24 11.4299 4.46999 11.2299 4.60999C11.0299 4.74999 10.7698 4.78001 10.5498 4.70001L9.87985 4.47Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M21 8L12 22L2.95996 8" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M3 4H6L12 13L18 4H21L12 18L3 4Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8 3L12 9L16 3L13.2 4V2H10.8V4L8 3Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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