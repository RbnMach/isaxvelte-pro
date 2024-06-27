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
<path d="M10 3L8 21" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16 3L14 21" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3.5 9H21.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M2.5 15H20.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M10.4199 13.4181H13.2599L13.5799 10.5781H10.7399L10.4199 13.4181Z" fill="{color}"/>
<path d="M16.19 2H7.81C4.17 2 2 4.17 2 7.81V16.18C2 19.83 4.17 22 7.81 22H16.18C19.82 22 21.99 19.83 21.99 16.19V7.81C22 4.17 19.83 2 16.19 2ZM18.82 10.58H15.05L14.73 13.43H18.1C18.5 13.43 18.83 13.76 18.83 14.16C18.83 14.56 18.5 14.89 18.1 14.89H14.57L14.16 18.55C14.12 18.92 13.8 19.2 13.43 19.2C13.4 19.2 13.38 19.2 13.35 19.2C12.95 19.16 12.66 18.79 12.7 18.39L13.09 14.89H10.25L9.84 18.55C9.8 18.92 9.48 19.2 9.11 19.2C9.08 19.2 9.06 19.2 9.03 19.2C8.63 19.16 8.34 18.79 8.38 18.39L8.77 14.89H5.18C4.78 14.89 4.45 14.56 4.45 14.16C4.45 13.76 4.78 13.43 5.18 13.43H8.95L9.27 10.58H5.9C5.5 10.58 5.17 10.25 5.17 9.85C5.17 9.45 5.5 9.12 5.9 9.12H9.43L9.84 5.46C9.88 5.06 10.25 4.77 10.65 4.81C11.05 4.85 11.34 5.22 11.3 5.62L10.91 9.12H13.75L14.16 5.46C14.21 5.06 14.57 4.77 14.97 4.81C15.37 4.85 15.66 5.22 15.62 5.62L15.23 9.12H18.84C19.24 9.12 19.57 9.45 19.57 9.85C19.57 10.25 19.22 10.58 18.82 10.58Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M10 3L8 21" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16 3L14 21" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M20.0508 9H21.5008" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3.5 9H16.99" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M3.95 15H2.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M20.4998 15H7.00977" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M16.19 2H7.81C4.17 2 2 4.17 2 7.81V16.18C2 19.83 4.17 22 7.81 22H16.18C19.82 22 21.99 19.83 21.99 16.19V7.81C22 4.17 19.83 2 16.19 2Z" fill="{color}"/>
<path d="M18.8192 10.5799C19.2192 10.5799 19.5492 10.25 19.5492 9.84995C19.5492 9.44995 19.2192 9.11995 18.8192 9.11995H15.2092L15.5992 5.61995C15.6392 5.21995 15.3592 4.85995 14.9492 4.80995C14.5492 4.76995 14.1892 5.04995 14.1392 5.45995L13.7292 9.11995H10.8992L11.2892 5.61995C11.3292 5.21995 11.0492 4.85995 10.6392 4.80995C10.2392 4.76995 9.87922 5.04995 9.82922 5.45995L9.42922 9.11995H5.89922C5.49922 9.11995 5.16922 9.44995 5.16922 9.84995C5.16922 10.25 5.49922 10.5799 5.89922 10.5799H9.26922L8.94922 13.43H5.17922C4.77922 13.43 4.44922 13.76 4.44922 14.16C4.44922 14.5599 4.77922 14.89 5.17922 14.89H8.78922L8.39922 18.3899C8.35922 18.7899 8.63922 19.15 9.04922 19.2C9.07922 19.2 9.09922 19.2 9.12922 19.2C9.49922 19.2 9.80922 18.9199 9.85922 18.5499L10.2692 14.89H13.1092L12.7192 18.3899C12.6792 18.7899 12.9592 19.15 13.3692 19.2C13.3992 19.2 13.4192 19.2 13.4492 19.2C13.8192 19.2 14.1292 18.9199 14.1792 18.5499L14.5892 14.89H18.1192C18.5192 14.89 18.8492 14.5599 18.8492 14.16C18.8492 13.76 18.5192 13.43 18.1192 13.43H14.7492L15.0692 10.5799H18.8192ZM13.2592 13.42H10.4192L10.7392 10.5699H13.5792L13.2592 13.42Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M7.99935 21.75C7.96935 21.75 7.93935 21.75 7.91935 21.75C7.50935 21.7 7.20935 21.33 7.25935 20.92L9.25935 2.92003C9.30935 2.51003 9.67935 2.22003 10.0894 2.26003C10.4994 2.31003 10.7994 2.68003 10.7494 3.09003L8.74935 21.09C8.69935 21.47 8.37935 21.75 7.99935 21.75Z" fill="{color}"/>
<path d="M13.9994 21.75C13.9694 21.75 13.9394 21.75 13.9194 21.75C13.5094 21.7 13.2094 21.33 13.2594 20.92L15.2594 2.92003C15.3094 2.51003 15.6694 2.22003 16.0894 2.26003C16.4994 2.31003 16.7994 2.68003 16.7494 3.09003L14.7494 21.09C14.6994 21.47 14.3794 21.75 13.9994 21.75Z" fill="{color}"/>
<path d="M21.5 9.75H3.5C3.09 9.75 2.75 9.41 2.75 9C2.75 8.59 3.09 8.25 3.5 8.25H21.5C21.91 8.25 22.25 8.59 22.25 9C22.25 9.41 21.91 9.75 21.5 9.75Z" fill="{color}"/>
<path d="M20.5 15.75H2.5C2.09 15.75 1.75 15.41 1.75 15C1.75 14.59 2.09 14.25 2.5 14.25H20.5C20.91 14.25 21.25 14.59 21.25 15C21.25 15.41 20.91 15.75 20.5 15.75Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M10 3L8 21" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M16 3L14 21" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M3.5 9H21.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M2.5 15H20.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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