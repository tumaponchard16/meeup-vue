<template>
	<v-alert error icon="warning" dismissible @input="onClose" :value="true">
      	{{ text }}
    </v-alert>
</template>

<script>
	/* eslint-disable */
	export default {
		props: ['text'],
		methods: {
			onClose () {
				this.$emit('dismissed')
			}
		}
	}
</script>
