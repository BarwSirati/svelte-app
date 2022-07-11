<script context="module" lang="ts">
	/** @type {import('@sveltejs/kit').Load} */
	import type { loadError, propsError } from '../lib/interfaces/loadError';
	export function load({ error, status }: loadError) {
		return {
			props: {
				title: `${status}: ${error.message}`
			}
		};
	}
</script>

<script lang="ts">
	export let title: string;
</script>

<h1>{title}</h1>
