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
<path d="M2.59991 3.60001L9.29991 20.4C9.69991 21.3 10.3999 21.4 10.9999 20.6L20.3999 8.70001C20.6999 8.30001 20.6999 7.70001 20.2999 7.40001L17.1999 4.30001C17.0999 4.10001 16.7999 4.00001 16.6999 4.00001L3.69991 2.30001C2.79991 2.10001 2.29991 2.70001 2.59991 3.60001Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M10 20.9999L11 9.9999L3 2.8999" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17 4L11 10L20 8.2" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M19.4016 10.5308C19.9216 10.4308 20.2816 11.0208 19.9616 11.4408L13.0116 20.2908C12.6616 20.7408 11.9416 20.4508 12.0016 19.8908L12.7016 12.2908C12.7216 12.0408 12.9115 11.8308 13.1615 11.7808L19.4016 10.5308Z" fill="{color}"/>
<path d="M21.6408 7.69118C21.8608 7.93118 21.7408 8.32118 21.4308 8.39118L12.9908 10.0812C12.4408 10.1912 12.0808 9.52118 12.4808 9.12118L17.5008 4.10118C17.7308 3.87118 18.1008 3.88118 18.3208 4.11118L21.6408 7.69118Z" fill="{color}"/>
<path d="M14.691 3.19104C15.161 3.25104 15.351 3.82104 15.021 4.16104L11.461 7.72104C11.251 7.93104 10.911 7.94104 10.681 7.74104L5.34104 2.99104C4.92104 2.62104 5.24099 1.93104 5.79099 2.00104L14.691 3.19104Z" fill="{color}"/>
<path d="M10.7207 10.0729C10.9907 10.3129 11.1207 10.6629 11.1007 11.0129L10.2407 21.4729C10.1907 22.0729 9.36076 22.1929 9.14076 21.6329L2.29072 3.96287C2.07072 3.40287 2.75076 2.93287 3.20076 3.33287L10.7207 10.0729Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M6.18992 12.4799L9.34989 20.3899C9.69989 21.2799 10.4799 21.3899 11.0599 20.6399L20.4399 8.69991C20.7399 8.31991 20.7099 7.71991 20.3599 7.37991L17.2299 4.24991C17.0999 4.11991 16.8399 3.98991 16.6599 3.96991L3.69993 2.22991C2.76993 2.10991 2.28993 2.71991 2.63993 3.58991L4.39994 7.99991" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M9.99976 20.9999L10.9998 9.9999L3.00977 2.8999" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17 4L11 10L20.04 8.19" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" d="M27.547 10.72c0 0.307-0.080 0.627-0.28 0.88l-12.507 15.92c-0.453 0.573-0.987 0.773-1.44 0.613l0.013-0.133 1.333-14.667 12.053-2.413 0.827-0.2z"></path>
<path fill="{color}" opacity="0.4" d="M27.547 10.72l-0.827 0.2-12.053 2.413 7.933-7.933c0.16 0.067 0.293 0.16 0.387 0.253l4.173 4.173c0.24 0.24 0.373 0.56 0.387 0.893z"></path>
<path fill="{color}" d="M22.6 5.4l-7.933 7.933-10.653-9.467-0.467-0.453v-0.013c0.267-0.347 0.747-0.52 1.387-0.427l17.28 2.307c0.12 0.013 0.253 0.053 0.387 0.12z"></path>
<path fill="{color}" opacity="0.4" d="M14.666 13.333l-1.333 14.667-0.013 0.133c-0.333-0.12-0.64-0.44-0.84-0.947l-8.96-22.4c-0.227-0.56-0.2-1.040 0.027-1.373l0.467 0.453 10.653 9.467z"></path>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M10.2302 21.8798C10.1602 21.8798 10.0903 21.8798 10.0203 21.8598C9.43026 21.7798 8.93022 21.3398 8.66022 20.6598L1.94025 3.85977C1.67025 3.18977 1.73027 2.53977 2.09027 2.06977C2.46027 1.59977 3.07022 1.37977 3.79022 1.47977L16.7603 3.20977C17.1103 3.25977 17.5203 3.45977 17.7703 3.70977L20.9003 6.83977C21.5103 7.45977 21.5802 8.46977 21.0402 9.15977L11.6602 21.0998C11.2602 21.6098 10.7502 21.8798 10.2302 21.8798ZM3.46027 2.95977C3.34027 2.95977 3.28026 2.98977 3.27026 2.99977C3.27026 3.00977 3.25026 3.11977 3.33026 3.30977L10.0502 20.1098C10.1302 20.3098 10.2202 20.3798 10.2302 20.3798C10.2402 20.3798 10.3402 20.3398 10.4702 20.1698L19.8502 8.22977C19.9202 8.14977 19.9103 7.96977 19.8303 7.89977L16.7003 4.76977C16.6803 4.74977 16.5902 4.70977 16.5502 4.69977L3.60022 2.96977C3.55022 2.95977 3.50027 2.95977 3.46027 2.95977Z" fill="{color}"/>
<path d="M10.0003 21.7498C9.98034 21.7498 9.95033 21.7498 9.93033 21.7498C9.52033 21.7098 9.21034 21.3498 9.25034 20.9398L10.2203 10.3198L2.51035 3.46976C2.20035 3.18976 2.17035 2.71976 2.45035 2.40976C2.73035 2.09976 3.20035 2.06976 3.51035 2.34976L11.5003 9.44976C11.6803 9.60976 11.7703 9.83976 11.7503 10.0798L10.7503 21.0798C10.7103 21.4598 10.3803 21.7498 10.0003 21.7498Z" fill="{color}"/>
<path d="M10.9998 10.7499C10.7298 10.7499 10.4699 10.5999 10.3399 10.3499C10.1799 10.0599 10.2398 9.69994 10.4698 9.46994L16.4698 3.46994C16.7598 3.17994 17.2399 3.17994 17.5299 3.46994C17.8199 3.75994 17.8199 4.23994 17.5299 4.52994L13.2799 8.77994L19.8898 7.45994C20.2998 7.37994 20.6899 7.63994 20.7699 8.04994C20.8499 8.45994 20.5898 8.84994 20.1798 8.92994L11.1398 10.7399C11.0998 10.7499 11.0498 10.7499 10.9998 10.7499Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M2.64012 3.58986L9.36009 20.3899C9.71009 21.2799 10.4901 21.3899 11.0701 20.6399L20.4501 8.69986C20.7501 8.31986 20.7201 7.71986 20.3701 7.37986L17.2401 4.24986C17.1101 4.11986 16.8501 3.98986 16.6701 3.96986L3.70011 2.22986C2.76011 2.09986 2.29012 2.70986 2.64012 3.58986Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<g opacity="0.4">
<path d="M9.99976 20.9999L10.9998 9.9999L3.00977 2.8999" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17 4L11 10L20.04 8.19" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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