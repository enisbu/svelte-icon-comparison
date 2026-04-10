<script lang="ts">
	import type { Snippet } from 'svelte';

	let {
		label,
		children,
		disabled = false
	}: { label: string; children?: Snippet; disabled?: boolean } = $props();
</script>

<div class="flex flex-col items-center gap-1.5">
	<div
		class="flex h-12 w-12 items-center justify-center rounded-xl {disabled
			? 'bg-zinc-800/40 text-zinc-600'
			: 'bg-zinc-800/80 transition-colors hover:bg-zinc-700/80'}"
	>
		{#if disabled}
			<span class="text-xs">N/A</span>
		{:else}
			{@render children?.()}
		{/if}
	</div>
	<span class="text-[10px] text-zinc-500">{label}</span>
</div>
