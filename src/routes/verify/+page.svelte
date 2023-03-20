<script>
	import { onMount } from 'svelte';

	let token = '';

	onMount(() => {
		token = new URLSearchParams(window.location.search).get('token');
	});
</script>

<h1>{token}</h1>
