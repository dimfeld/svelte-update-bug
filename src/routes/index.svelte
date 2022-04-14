<script>
	import Comp from './_Comp.svelte';
	import CWrapper from './_CWrapper.svelte';
	import Hello from './_Hello.svelte';
	import Another from './_Another.svelte';
	import { writable } from 'svelte/store';
	import { setContext } from 'svelte';
 
	let s = writable(false);
	
	setContext('storevalue', s);
</script>

<div>
	<Hello />
	<CWrapper Component={Comp} />
	<Another />
</div>
