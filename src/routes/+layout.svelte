<script>
	import '../app.css';
	import Header from '$lib/components/molecules/Header.svelte';
	import Divider from '$lib/components/atoms/Divider.svelte';
</script>

<Header />
<Divider />
<div class="p-2">
	<slot />
</div>
