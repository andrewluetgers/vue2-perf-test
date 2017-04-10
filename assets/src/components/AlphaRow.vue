<template>
	<ul key="$index">
		<slot></slot>
	</ul>
</template>

<script>
	import AlphaCell from './AlphaCell.vue'

	export default {
		name: "AlphaRow",
		components: {AlphaCell},
		props: ['row']
	}
</script>