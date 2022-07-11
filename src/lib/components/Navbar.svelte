<script>
	import { each } from 'svelte/internal';

	const configPaths = [
		{ to: '/', name: 'Home' },
		{ to: 'todos', name: 'Todos' }
	];
</script>

<nav class="w-full bg-slate-900 p-5 flex text-white font-semibold">
	<div class="mr-auto"><h1 class="text-2xl">TodoList</h1></div>
	<div class="ml-auto">
		<ul class="flex space-x-5">
			{#each configPaths as configPath}
				<a href={configPath.to}><li>{configPath.name}</li></a>
			{/each}
		</ul>
	</div>
</nav>
