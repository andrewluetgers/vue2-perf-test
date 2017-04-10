<template>
    <div id="alphaTable">
        <ul key="$index" v-for="row in layout">
			<alpha-cell v-for="cell in row" :cell="cell"></alpha-cell>
		</ul>
    </div>
</template>

<script>
	import AlphaCell from './AlphaCell.vue'

	export default {
		components: {AlphaCell},
        props: ['layout']
    }
</script>


<style lang="stylus" rel="stylesheet/stylus">
    #alphaTable
        margin-top 20px
        width 400px

        ul
            padding 0
            margin 0
            display table-row
            background green
            transform scale(1)

            li
                display table-cell
                padding 0
                margin 0
                font-size 0
                width 4px
                height 4px
                line-height 4px
                overflow hidden
                background blue

                &.active
                    background yellow

                &.inactive
                    background white
</style>