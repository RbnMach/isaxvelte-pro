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
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6.6001 9.3001C10.2001 7.9001 14.3001 8.4001 17.5001 10.6001" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7.8999 12.4C10.5999 11.4 13.5999 11.7 15.8999 13.4" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.80005 15.4001C10.8 14.6001 13 14.9001 14.8 16.1001" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}
	{#if type == 'bold'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM15.42 16.58C15.27 16.79 15.04 16.89 14.81 16.89C14.66 16.89 14.51 16.84 14.37 16.75C12.83 15.65 10.86 15.41 9.10001 16.1C8.72001 16.25 8.28 16.06 8.13 15.68C7.98 15.29 8.17 14.86 8.55 14.71C10.79 13.82 13.29 14.13 15.24 15.53C15.59 15.78 15.66 16.25 15.42 16.58ZM16.52 13.79C16.37 14 16.14 14.1 15.91 14.1C15.76 14.1 15.61 14.05 15.47 13.96C13.35 12.44 10.64 12.11 8.21001 13.07C7.83001 13.22 7.39001 13.03 7.24001 12.65C7.09001 12.26 7.28 11.83 7.66 11.68C10.56 10.53 13.81 10.93 16.34 12.75C16.68 12.99 16.76 13.46 16.52 13.79ZM18.09 11.11C17.94 11.32 17.71 11.42 17.48 11.42C17.33 11.42 17.18 11.37 17.04 11.28C14.06 9.14 10.24 8.67 6.84 10.03C6.45 10.18 6.02 9.98999 5.87 9.60999C5.72 9.22999 5.90999 8.79001 6.28999 8.64001C10.17 7.10001 14.52 7.63001 17.92 10.07C18.26 10.3 18.34 10.77 18.09 11.11Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'broken'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M6.57031 9.33007C10.2003 7.89007 14.3103 8.40009 17.4903 10.6701" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M7.93945 12.3801C10.5895 11.3301 13.5895 11.7001 15.9095 13.3601" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8.83008 15.4099C10.8201 14.6199 13.0701 14.9 14.8101 16.14" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M4 6C2.75 7.67 2 9.75 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2C10.57 2 9.2 2.30001 7.97 2.85001" stroke="{color}" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

	{/if}										
	{#if type == 'bulk'}
		<svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
<path fill="{color}" opacity="0.4" d="M16 29.333c7.364 0 13.333-5.97 13.333-13.333s-5.97-13.333-13.333-13.333c-7.364 0-13.333 5.97-13.333 13.333s5.97 13.333 13.333 13.333z"></path>
<path fill="{color}" d="M23.306 15.227c-0.2 0-0.4-0.067-0.587-0.187-3.973-2.853-9.067-3.48-13.6-1.667-0.52 0.2-1.093-0.053-1.293-0.56s0.053-1.093 0.56-1.293c5.173-2.053 10.973-1.347 15.507 1.907 0.453 0.32 0.547 0.947 0.227 1.4-0.187 0.253-0.493 0.4-0.813 0.4z"></path>
<path fill="{color}" d="M21.214 18.814c-0.2 0-0.4-0.067-0.587-0.187-2.827-2.027-6.44-2.467-9.68-1.187-0.507 0.2-1.093-0.053-1.293-0.56-0.2-0.52 0.053-1.093 0.56-1.293 3.867-1.533 8.2-1 11.573 1.427 0.453 0.32 0.547 0.947 0.227 1.4-0.187 0.253-0.493 0.4-0.8 0.4z"></path>
<path fill="{color}" d="M19.746 22.533c-0.2 0-0.4-0.067-0.587-0.187-2.053-1.467-4.68-1.787-7.027-0.867-0.507 0.2-1.093-0.053-1.293-0.56-0.2-0.52 0.053-1.093 0.56-1.293 2.987-1.187 6.32-0.773 8.92 1.093 0.453 0.32 0.547 0.947 0.227 1.4-0.173 0.267-0.48 0.413-0.8 0.413z"></path>
</svg>

	{/if}										
	{#if type == 'outline'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12C1.25 6.07 6.07 1.25 12 1.25C17.93 1.25 22.75 6.07 22.75 12C22.75 17.93 17.93 22.75 12 22.75ZM12 2.75C6.9 2.75 2.75 6.9 2.75 12C2.75 17.1 6.9 21.25 12 21.25C17.1 21.25 21.25 17.1 21.25 12C21.25 6.9 17.1 2.75 12 2.75Z" fill="{color}"/>
<path d="M17.4797 11.4202C17.3297 11.4202 17.1797 11.3701 17.0397 11.2801C14.0597 9.14014 10.2397 8.67014 6.83973 10.0301C6.44973 10.1801 6.01973 9.99013 5.86973 9.61013C5.71973 9.23013 5.90973 8.79016 6.28973 8.64016C10.1697 7.10016 14.5197 7.63015 17.9197 10.0701C18.2597 10.3101 18.3297 10.7801 18.0897 11.1201C17.9497 11.3101 17.7197 11.4202 17.4797 11.4202Z" fill="{color}"/>
<path d="M15.9098 14.1102C15.7598 14.1102 15.6098 14.0602 15.4698 13.9702C13.3498 12.4502 10.6399 12.1202 8.20985 13.0802C7.82985 13.2302 7.38985 13.0402 7.23985 12.6602C7.08985 12.2702 7.27985 11.8402 7.65985 11.6902C10.5598 10.5402 13.8098 10.9402 16.3398 12.7602C16.6798 13.0002 16.7498 13.4702 16.5098 13.8102C16.3698 14.0002 16.1398 14.1102 15.9098 14.1102Z" fill="{color}"/>
<path d="M14.8105 16.9C14.6605 16.9 14.5105 16.8501 14.3705 16.7601C12.8305 15.6601 10.8605 15.42 9.10048 16.11C8.72048 16.26 8.28047 16.0701 8.13047 15.6901C7.98047 15.3001 8.17047 14.8701 8.55047 14.7201C10.7905 13.8301 13.2905 14.1401 15.2405 15.5401C15.5805 15.7801 15.6505 16.2501 15.4105 16.5901C15.2805 16.7901 15.0505 16.9 14.8105 16.9Z" fill="{color}"/>
</svg>

	{/if}										
	{#if type == 'twotone'}
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M6.57031 9.32982C10.2003 7.88982 14.3103 8.39985 17.4903 10.6698" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M7.94043 12.3801C10.5904 11.3301 13.5904 11.7001 15.9104 13.3601" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
<path opacity="0.4" d="M8.83008 15.4099C10.8201 14.6199 13.0701 14.9 14.8101 16.14" stroke="{color}" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
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