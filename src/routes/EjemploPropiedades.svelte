<script lang="ts">
	import Bank from '$lib/Bank.svelte';
</script>

<p>
	<Bank
		variant="bulk"
		size="2em"
		axis_x="5px"
		axis_y="-10px"
		color="rgb(255, 55, 0)"
		rotate={15}
	/>Bank
</p>

<style>
	p {
		font-size: 28px;
		color: rgb(155, 57, 38);
	}
</style>
