<script lang="ts">
	import { createEventDispatcher } from 'svelte'

	const dispatch = createEventDispatcher()

	function handleMouseMove(event) {
		dispatch('updatePosition', event)
	}
</script>

<div class="mousearea" on:mousemove={handleMouseMove} />
