<script>
	import { getContext } from 'svelte';
	const s = getContext('storevalue');
</script>

	{#if $s}
		<h1>Another</h1>

	{/if}

