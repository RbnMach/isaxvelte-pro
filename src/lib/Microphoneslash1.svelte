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
<path d="M17.82 6.53C17.16 3.93 14.81 2 12 2C8.69 2 6 4.69 6 8V13C6 14.46 6.52 15.8 7.39 16.84" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17.9999 9.97998V13C17.9999 16.31 15.3099 19 11.9999 19C11.2699 19 10.5599 18.87 9.91992 18.63" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5.86011 19.58C7.47011 21.08 9.63011 22 12.0001 22C16.9701 22 21.0001 17.97 21.0001 13V11" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M21.5 2.98999L2.5 21.99" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.55 5.50001V2.26001" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.5 3.5V7.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if variant == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M17.6189 5.72L7.00891 16.33C6.27891 15.34 5.87891 14.13 5.87891 12.82V8.11C5.87891 6.27 6.69891 4.62 7.99891 3.5V7.64C7.99891 8.03 8.31891 8.35 8.69891 8.35C9.08891 8.35 9.40891 8.03 9.40891 7.64V2.57C9.86891 2.34 10.3589 2.18 10.8689 2.09V5.75C10.8689 6.15 11.1889 6.46 11.5789 6.46C11.9689 6.46 12.2889 6.15 12.2889 5.75V2C14.6789 2.11 16.7389 3.61 17.6189 5.72Z" fill="{color}"/>
<path d="M18.1202 8.87891V12.8189C18.1202 16.1889 15.3702 18.9389 12.0002 18.9389C11.8202 18.9389 11.6402 18.9289 11.4602 18.9089C11.3802 18.9089 11.3002 18.8989 11.2302 18.8889C11.1002 18.8689 10.9702 18.8489 10.8502 18.8289C10.8002 18.8289 10.7602 18.8089 10.7002 18.7989C10.5602 18.7689 10.4202 18.7289 10.2902 18.6889C10.0702 18.6289 9.86016 18.5489 9.66016 18.4689C9.53016 18.4189 9.41016 18.3689 9.29016 18.2989C9.26016 18.2889 9.24016 18.2689 9.21016 18.2589C9.11016 18.2089 9.01016 18.1589 8.91016 18.0889L18.1202 8.87891Z" fill="{color}"/>
<path d="M21.7497 11V13C21.7497 18.38 17.3797 22.75 11.9997 22.75C9.87969 22.75 7.84969 22.07 6.17969 20.82L7.25969 19.74C8.63969 20.72 10.2797 21.25 11.9997 21.25C16.5497 21.25 20.2497 17.55 20.2497 13V11C20.2497 10.59 20.5897 10.25 20.9997 10.25C21.4097 10.25 21.7497 10.59 21.7497 11Z" fill="{color}"/>
<path d="M21.7689 2.22891C21.4689 1.92891 20.9789 1.92891 20.6789 2.22891L2.22891 20.6889C1.92891 20.9889 1.92891 21.4789 2.22891 21.7789C2.37891 21.9189 2.56891 21.9989 2.76891 21.9989C2.96891 21.9989 3.15891 21.9189 3.30891 21.7689L21.7689 3.30891C22.0789 3.00891 22.0789 2.52891 21.7689 2.22891Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M6 12V13C6 14.46 6.52 15.8 7.39 16.84" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17.82 6.53C17.16 3.93 14.81 2 12 2C8.69 2 6 4.69 6 8" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M17.9999 9.97998V13C17.9999 16.31 15.3099 19 11.9999 19C11.2699 19 10.5599 18.87 9.91992 18.63" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M5.85938 19.58C7.46938 21.08 9.62937 22 11.9994 22C16.9694 22 20.9994 17.97 20.9994 13V11" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M21.5 2.99023L2.5 21.9902" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.5508 5.49977V2.25977" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.5 3.5V7.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if variant == 'bulk'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path opacity="0.4" d="M17.6209 5.72L7.01086 16.33C6.28086 15.34 5.88086 14.13 5.88086 12.82V8.11C5.88086 6.27 6.70086 4.62 8.00086 3.5V7.64C8.00086 8.03 8.32086 8.35 8.70086 8.35C9.09086 8.35 9.41086 8.03 9.41086 7.64V2.57C9.87086 2.34 10.3609 2.18 10.8709 2.09V5.75C10.8709 6.15 11.1909 6.46 11.5809 6.46C11.9709 6.46 12.2909 6.15 12.2909 5.75V2C14.6809 2.11 16.7409 3.61 17.6209 5.72Z" fill="{color}"/>
<path d="M18.1202 8.87988V12.8199C18.1202 16.1899 15.3702 18.9399 12.0002 18.9399C11.8202 18.9399 11.6402 18.9299 11.4602 18.9099C11.3802 18.9099 11.3002 18.8999 11.2302 18.8899C11.1002 18.8699 10.9702 18.8499 10.8502 18.8299C10.8002 18.8299 10.7602 18.8099 10.7002 18.7999C10.5602 18.7699 10.4202 18.7299 10.2902 18.6899C10.0702 18.6299 9.86016 18.5499 9.66016 18.4699C9.53016 18.4199 9.41016 18.3699 9.29016 18.2999C9.26016 18.2899 9.24016 18.2699 9.21016 18.2599C9.11016 18.2099 9.01016 18.1599 8.91016 18.0899L18.1202 8.87988Z" fill="{color}"/>
<path d="M21.7497 11V13C21.7497 18.38 17.3797 22.75 11.9997 22.75C9.87969 22.75 7.84969 22.07 6.17969 20.82L7.25969 19.74C8.63969 20.72 10.2797 21.25 11.9997 21.25C16.5497 21.25 20.2497 17.55 20.2497 13V11C20.2497 10.59 20.5897 10.25 20.9997 10.25C21.4097 10.25 21.7497 10.59 21.7497 11Z" fill="{color}"/>
<path d="M21.7709 2.22988C21.4709 1.92988 20.9809 1.92988 20.6809 2.22988L2.23086 20.6899C1.93086 20.9899 1.93086 21.4799 2.23086 21.7799C2.38086 21.9199 2.57086 21.9999 2.77086 21.9999C2.97086 21.9999 3.16086 21.9199 3.31086 21.7699L21.7709 3.30988C22.0809 3.00988 22.0809 2.52988 21.7709 2.22988Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M7.39 17.59C7.18 17.59 6.96 17.5 6.81 17.32C5.8 16.11 5.25 14.58 5.25 13V8C5.25 4.28 8.28 1.25 12 1.25C15.1 1.25 17.79 3.35 18.55 6.35C18.65 6.75 18.41 7.16 18.01 7.26C17.62 7.36 17.2 7.12 17.1 6.72C16.5 4.38 14.41 2.75 12 2.75C9.11 2.75 6.75 5.1 6.75 8V13C6.75 14.23 7.18 15.42 7.96 16.36C8.23 16.68 8.18 17.15 7.86 17.42C7.73 17.53 7.56 17.59 7.39 17.59Z" fill="{color}"/>
<path d="M11.9998 19.75C11.1898 19.75 10.3998 19.61 9.65984 19.33C9.26984 19.19 9.06984 18.75 9.21984 18.37C9.35984 17.98 9.79984 17.78 10.1798 17.93C10.7598 18.15 11.3798 18.26 11.9998 18.26C14.8898 18.26 17.2498 15.91 17.2498 13.01V9.97998C17.2498 9.56998 17.5898 9.22998 17.9998 9.22998C18.4098 9.22998 18.7498 9.56998 18.7498 9.97998V13C18.7498 16.72 15.7198 19.75 11.9998 19.75Z" fill="{color}"/>
<path d="M11.9994 22.7502C9.51941 22.7502 7.15941 21.8202 5.34941 20.1302C5.04941 19.8502 5.02941 19.3702 5.30941 19.0702C5.58941 18.7702 6.06941 18.7502 6.36941 19.0302C7.89941 20.4602 9.89941 21.2402 11.9894 21.2402C16.5394 21.2402 20.2394 17.5402 20.2394 12.9902V10.9902C20.2394 10.5802 20.5794 10.2402 20.9894 10.2402C21.3994 10.2402 21.7394 10.5802 21.7394 10.9902V12.9902C21.7494 18.3802 17.3794 22.7502 11.9994 22.7502Z" fill="{color}"/>
<path d="M2.49945 22.7402C2.30945 22.7402 2.11945 22.6702 1.96945 22.5202C1.67945 22.2302 1.67945 21.7502 1.96945 21.4602L20.9695 2.46018C21.2595 2.17018 21.7395 2.17018 22.0295 2.46018C22.3195 2.75018 22.3195 3.23018 22.0295 3.52018L3.02945 22.5202C2.87945 22.6702 2.68945 22.7402 2.49945 22.7402Z" fill="{color}"/>
<path d="M11.5508 6.24977C11.1408 6.24977 10.8008 5.90977 10.8008 5.49977V2.25977C10.8008 1.84977 11.1408 1.50977 11.5508 1.50977C11.9608 1.50977 12.3008 1.84977 12.3008 2.25977V5.49977C12.3008 5.91977 11.9608 6.24977 11.5508 6.24977Z" fill="{color}"/>
<path d="M8.5 8.25C8.09 8.25 7.75 7.91 7.75 7.5V3.5C7.75 3.09 8.09 2.75 8.5 2.75C8.91 2.75 9.25 3.09 9.25 3.5V7.5C9.25 7.91 8.91 8.25 8.5 8.25Z" fill="{color}"/>
</svg>

	{/if}										
	{#if variant == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M17.82 6.53C17.16 3.93 14.81 2 12 2C8.69 2 6 4.69 6 8V13C6 14.46 6.52 15.8 7.39 16.84" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M17.9999 9.97998V13C17.9999 16.31 15.3099 19 11.9999 19C11.2699 19 10.5599 18.87 9.91992 18.63" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M5.85938 19.58C7.46938 21.08 9.62937 22 11.9994 22C16.9694 22 20.9994 17.97 20.9994 13V11" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M21.5 2.99023L2.5 21.9902" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M11.5508 5.49977V2.25977" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.5 3.5V7.5" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
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