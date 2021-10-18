<template>
	<div class="hello">
		<vue-qr :logoSrc="imageUrl" text="123456" :size="200"></vue-qr>
	</div>
</template>

<script>
	import vueQr from 'vue-qr'
	export default {
		name: 'HelloWorld',
		data() {
			return {
				imageUrl: require("../assets/logo.png"),
			}
		},
		props: {
			msg: String
		},
		components: {
			vueQr
		},
	}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
	h3 {
		margin: 40px 0 0;
	}

	ul {
		list-style-type: none;
		padding: 0;
	}

	li {
		display: inline-block;
		margin: 0 10px;
	}

	a {
		color: #42b983;
	}
</style>
