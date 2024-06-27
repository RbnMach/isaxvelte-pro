<script lang="ts">
	export let classes = '';
	export let color = 'currentColor';
	export let type: 'linear' | 'bold' | 'broken' | 'bulk' | 'outline' | 'twotone' = 'linear';
	export let size = '1em';
	export let axis_y = '-0.13em';
	export let axis_x = '0';
</script>

<span style="width: {size}; height: {size}; bottom: {axis_y}; left: {axis_x};" class={classes}>
	{#if type == 'linear'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15.1999 3H8.7999L1.3999 15.7L4.5999 21H19.3999C19.3999 21 22.5999 15.5 22.5999 15.6C22.5999 15.7 15.1999 3 15.1999 3Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.7998 3L19.3998 21" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.2001 3L4.6001 21" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M1.5 15.7H22" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5.94062 16.7712L4.28065 19.5912C4.16065 19.8012 3.85059 19.8012 3.72059 19.5912L2.03065 16.7712C1.90065 16.5512 2.06062 16.2812 2.31062 16.2812H5.66059C5.91059 16.2812 6.06062 16.5612 5.94062 16.7712Z" fill="{color}"/>
<path d="M11.6904 8.40844L7.7404 14.8784C7.6504 15.0284 7.49041 15.1084 7.32041 15.1084H2.25041C1.87041 15.1084 1.63041 14.7085 1.82041 14.3885L8.28043 3.72845C8.47043 3.41845 8.94041 3.40845 9.13041 3.72845L11.6904 7.93844C11.7804 8.07844 11.7804 8.25844 11.6904 8.40844Z" fill="{color}"/>
<path d="M13.721 14.4892H10.241C10.041 14.4892 9.91104 14.2692 10.011 14.0892L11.751 11.1392C11.851 10.9692 12.101 10.9692 12.201 11.1392L13.941 14.0892C14.051 14.2692 13.921 14.4892 13.721 14.4892Z" fill="{color}"/>
<path d="M13.6614 3.39999L12.2114 5.87C12.1114 6.04 11.8514 6.04 11.7514 5.87L10.3014 3.39999C10.2014 3.21999 10.3215 3 10.5315 3H13.4314C13.6414 3 13.7614 3.21999 13.6614 3.39999Z" fill="{color}"/>
<path d="M22.1695 14.3684C22.3695 14.6984 22.1195 15.1184 21.7395 15.1184H16.8695C16.6995 15.1184 16.5495 15.0285 16.4595 14.8885L12.6495 8.41845C12.5595 8.26845 12.5595 8.08844 12.6495 7.93844L15.1195 3.72845C15.2995 3.41845 15.7595 3.40845 15.9395 3.72845C17.1595 5.83845 20.8895 12.1784 22.1695 14.3684Z" fill="{color}"/>
<path d="M21.9307 16.7695C21.3807 17.6995 20.7907 18.6995 20.2507 19.6095C20.1207 19.8295 19.8107 19.8195 19.6807 19.5995L18.0207 16.7695C17.8907 16.5495 18.0507 16.2695 18.3107 16.2695H21.6407C21.9007 16.2795 22.0607 16.5495 21.9307 16.7695Z" fill="{color}"/>
<path d="M18.0207 20.9994H5.94068C5.58068 20.9994 5.36065 20.6094 5.54065 20.2994L7.87067 16.3394C7.95067 16.1994 8.10069 16.1094 8.27069 16.1094H15.6907C15.8507 16.1094 16.0107 16.1994 16.0907 16.3394L18.4207 20.2994C18.6007 20.6094 18.3807 20.9994 18.0207 20.9994Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5.47015 8.73999L1.41016 15.7L4.59021 20.99H19.4102C19.4102 20.99 22.5902 15.54 22.5902 15.62C22.5902 15.7 15.1802 3 15.1802 3H8.8302L7.67017 4.98999" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.82031 3L19.4103 21" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.1798 3L4.58984 21" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M1.5 15.71H22" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M10.267 20.947l-4.147 7.053-4.24-7.053h8.387z"></path>
<path fill="{color}" d="M16 11.213l-5.733 9.733h-8.387l9.88-16.947 4.24 7.213z"></path>
<path fill="{color}" opacity="0.4" d="M20.24 4l-4.24 7.213-4.24-7.213h8.48z"></path>
<path fill="{color}" d="M30.12 20.84c0 0-0.027 0.040-0.080 0.107h-8.307l-5.733-9.733 4.24-7.213c0 0 9.813 16.84 9.88 16.84z"></path>
<path fill="{color}" opacity="0.4" d="M30.041 20.947c-0.56 0.88-4.16 7.053-4.16 7.053l-4.147-7.053h8.307z"></path>
<path fill="{color}" d="M25.88 28h-19.76l4.147-7.053h11.467l4.147 7.053z"></path>
<path fill="{color}" opacity="0.4" d="M21.732 20.947h-11.467l5.733-9.733 5.733 9.733z"></path>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M19.41 21.7498H4.59005C4.33005 21.7498 4.08003 21.6098 3.95003 21.3898L0.770039 16.0998C0.630039 15.8698 0.630039 15.5698 0.770039 15.3398L8.18001 2.62976C8.31001 2.39976 8.56004 2.25977 8.83004 2.25977H15.18C15.45 2.25977 15.69 2.39976 15.83 2.62976C18.62 7.40976 22.83 14.6197 23.19 15.1797C23.29 15.3097 23.34 15.4598 23.34 15.6298C23.34 15.8098 23.28 15.9698 23.17 16.0998C22.91 16.4898 21.15 19.5198 20.06 21.3798C19.93 21.6098 19.68 21.7498 19.41 21.7498ZM5.01003 20.2498H18.98C20.47 17.6898 21.27 16.3297 21.76 15.6097C21.19 14.7697 20.19 13.0698 18.22 9.69977L14.75 3.74976H9.26003L2.29 15.6998L5.01003 20.2498ZM22.37 16.3297V16.3498V16.3297Z" fill="{color}"/>
<path d="M19.4097 21.7499C19.1497 21.7499 18.8998 21.6199 18.7598 21.3799L8.16973 3.37992C7.95973 3.01992 8.07975 2.55992 8.43975 2.34992C8.79975 2.13992 9.25972 2.25991 9.46972 2.61991L20.0597 20.6199C20.2697 20.9799 20.1497 21.4399 19.7897 21.6499C19.6697 21.7199 19.5397 21.7499 19.4097 21.7499Z" fill="{color}"/>
<path d="M4.59027 21.7499C4.46027 21.7499 4.33026 21.7199 4.21026 21.6499C3.85026 21.4399 3.73024 20.9799 3.94024 20.6199L14.5303 2.61991C14.7403 2.25991 15.2002 2.13992 15.5602 2.34992C15.9202 2.55992 16.0403 3.01992 15.8303 3.37992L5.24023 21.3799C5.09023 21.6199 4.84027 21.7499 4.59027 21.7499Z" fill="{color}"/>
<path d="M22 16.46H1.5C1.09 16.46 0.75 16.12 0.75 15.71C0.75 15.3 1.09 14.96 1.5 14.96H22C22.41 14.96 22.75 15.3 22.75 15.71C22.75 16.12 22.41 16.46 22 16.46Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15.1799 3H8.82996L1.41992 15.71L4.59991 21H19.4199C19.4199 21 22.5999 15.55 22.5999 15.63C22.5999 15.71 15.1799 3 15.1799 3Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<g opacity="0.4">
<path d="M8.82031 3L19.4103 21" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M15.1798 3L4.58984 21" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M1.5 15.71H22" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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
</style>