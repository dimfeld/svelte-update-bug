<script>
	import { getContext, onMount, tick } from 'svelte';
	
	const s = getContext('storevalue');
	
	$s = true;

	// Doing this instead works around the problem
	// 	tick().then(() => $s = true)	
</script>
<h3>
	Hi
</h3>
