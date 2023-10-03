<script lang="ts">
	export let collapsed = false;
</script>

<div>
	{#if !collapsed}
		<svelte:self let:something>
			<slot {something} />
		</svelte:self>
	{/if}
</div>
