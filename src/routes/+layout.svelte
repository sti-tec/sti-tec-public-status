<script lang="ts">
	import '../app.css';
	import { browser } from '$app/environment';
	let { children } = $props();

	const FIVE_MINUTES = 300000;

	if (browser) {
		setTimeout(function(){
    		window.location.reload()
  		}, FIVE_MINUTES)
	}
</script>

{@render children()}
