<script lang="ts">
	export let catalogue: string[];
	export let onselect: (a: string) => {};
</script>

<div class="font-semibold capitalize flex flex-col gap-2 items-stretch text-center">
	{#each catalogue as item}
		<p class="btn px-6 pl-10" on:click={() => onselect(item)}>
			{item}
		</p>
	{/each}
</div>
