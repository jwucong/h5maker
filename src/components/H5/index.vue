<template>
	<div class="h5">
		<component
			v-for="module in modules"
			:is="module.component"
			:key="module.id"
			:data="module.data"
		>
		</component>
	</div>
</template>

<script>
export default {
	name: 'H5',
	props: {
		data: {
			types: Object,
			default: () => ({})
		}
	},
	computed: {
		modules() {
			return this.data.components || []
		}
	}
}
</script>

<style lang="scss" scoped></style>
