<script>
	import '../app.css';
	import Navbar from '../lib/components/Navbar.svelte';
</script>

<Navbar />
<div class="w-full p-5">
	<slot />
</div>
