<script>
	import { getContext } from 'svelte';
	const s = getContext('storevalue');
</script>

	{#if $s}
		<h1>Hello</h1>

	{/if}

