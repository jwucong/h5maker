<template>
	<div class="home">
		<HelloWorld msg="Welcome to Your Vue.js App" />
	</div>
</template>

<script>
// @ is an alias to /src
import H5 from '@/components/H5'

export default {
	name: 'home',
	components: {
		H5
	}
}
</script>
