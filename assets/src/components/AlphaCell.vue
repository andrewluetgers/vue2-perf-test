<template>
	<li key="$index" :style="{background: cell.active ? cell.color : '#444444'}">test</li>
</template>

<script>
	export default {
		name: "AlphaCell",
		props: ['cell']
	}
</script>