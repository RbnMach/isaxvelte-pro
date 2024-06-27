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
<path d="M12.7 11.7L16.8 15.8C17.3 16.4 17.1 17.3 16.4 17.6L6.10002 21.9C5.00002 22.4 4.10002 21 4.90002 20.2L12.7 11.7ZM12.7 11.7L8.60002 7.59995C8.10002 7.09995 8.30002 6.09995 9.00002 5.79995L17.9 2.09995C19 1.69995 19.9 2.89995 19.2 3.79995L12.7 11.7Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16.3794 17.5692L6.07939 21.9092C5.00939 22.3592 4.07937 21.0292 4.86937 20.1792L12.6794 11.6992L16.7294 15.8192C17.2694 16.3592 17.0894 17.2792 16.3794 17.5692Z" fill="{color}"/>
<path d="M19.171 3.77114L12.681 11.7011L8.63101 7.60114C8.09101 7.05114 8.27099 6.13114 8.98099 5.84114L17.921 2.09114C18.961 1.65114 19.891 2.90114 19.171 3.77114Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12.6795 11.6999L19.1695 3.76992C19.8795 2.89992 18.9495 1.64992 17.9095 2.08992L8.9695 5.83992C8.2595 6.13992 8.07953 7.04992 8.61953 7.59992L9.89956 8.89992M6.07955 21.9099L16.3795 17.5699C17.0895 17.2699 17.2695 16.3599 16.7295 15.8099L12.6695 11.6999L4.85952 20.1799C4.07952 21.0299 5.00955 22.3599 6.07955 21.9099Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M21.841 23.427l-13.733 5.787c-1.427 0.6-2.667-1.173-1.613-2.307l10.413-11.307 5.4 5.493c0.72 0.72 0.48 1.947-0.467 2.333z"></path>
<path fill="{color}" d="M25.56 5.027l-8.653 10.573-5.4-5.467c-0.72-0.733-0.48-1.96 0.467-2.347l11.92-5c1.387-0.587 2.627 1.080 1.667 2.24z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5.64043 22.7498C5.06043 22.7498 4.52039 22.4698 4.16039 21.9598C3.65039 21.2398 3.71042 20.3098 4.31042 19.6698L11.6404 11.7098L8.09044 8.11977C7.66044 7.68977 7.48039 7.06977 7.60039 6.46977C7.72039 5.86977 8.13042 5.37977 8.69042 5.13977L17.6304 1.38977C18.4204 1.05977 19.2904 1.29977 19.8104 1.97977C20.3204 2.66977 20.3004 3.56977 19.7604 4.23977L13.6904 11.6498L17.2704 15.2798C17.7004 15.7098 17.8804 16.3298 17.7604 16.9298C17.6404 17.5298 17.2304 18.0198 16.6704 18.2598L6.37041 22.5998C6.13041 22.6998 5.89043 22.7498 5.64043 22.7498ZM12.6904 12.7898L5.4204 20.6898C5.2604 20.8598 5.34043 21.0198 5.39043 21.1098C5.45043 21.1898 5.5804 21.3198 5.7904 21.2198L16.0904 16.8798C16.2304 16.8198 16.2704 16.6998 16.2904 16.6398C16.3004 16.5798 16.3104 16.4498 16.2004 16.3398L12.6904 12.7898ZM9.16039 7.06977L12.6304 10.5798L18.5904 3.29977C18.7304 3.12977 18.6604 2.96977 18.6004 2.88977C18.5404 2.80977 18.4204 2.68977 18.2004 2.77977L9.26043 6.52977C9.12043 6.58977 9.08042 6.70977 9.06042 6.76977C9.04042 6.82977 9.06039 6.95977 9.16039 7.06977Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M6.07955 21.9102L16.3795 17.5702C17.0895 17.2702 17.2695 16.3602 16.7295 15.8102L12.6695 11.7002L4.85952 20.1802C4.07952 21.0302 5.00955 22.3602 6.07955 21.9102ZM8.62954 7.60016L12.6795 11.7002L19.1695 3.77016C19.8795 2.90016 18.9495 1.65016 17.9095 2.09016L8.9695 5.84016C8.2695 6.13016 8.08954 7.05016 8.62954 7.60016Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10"/>
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