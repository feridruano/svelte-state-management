<script lang="ts">
	import Production, { bananas } from './production.svelte'
</script>

<Production />
<Production />

{#if $bananas.length}
	<div>{$bananas.join('')}</div>
{/if}
