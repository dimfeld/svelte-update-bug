<script>
  import { getAllContexts } from 'svelte';
	export let Component;
      const ctx = getAllContexts();

	function createWithClientApi(node) {
		const c = new Component({
                  target: node,
                  context: ctx,
		})
		return {
			destroy() {
				c.$destroy(); 
			}
		}
	}
</script>

<div style="display:contents" use:createWithClientApi />
