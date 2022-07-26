<script>
	import Nav from '/src/assets/Nav.svelte';
	import Footer from '/src/assets/Footer.svelte';
</script>

<body>
	<Nav />
	<slot />

	<Footer />
</body>

<style lang="scss">
	@import 'components';

	.footer {
		background: $gradient;

		h1 {
			margin: 5%;
		}

		ul {
			margin: 5%;
			list-style: none;

			li {
				margin: 1%;
				padding: 1%;
			}
		}
	}
</style>
