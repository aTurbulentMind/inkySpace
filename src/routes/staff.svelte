<body>
	<h1>Our staff</h1>
	<p>Some of the best people in the world call this place home.</p>
	<staff>
		<person>
			<a href="/bonnie">
				<img src="img/purp.png" alt="" />

				<h1>Bonnie <br /></h1></a
			>
		</person>
		<person>
			<a href="/">
				<img src="img/purp.png" alt="" />

				<h1>Jessie <br /></h1></a
			>
		</person>

		<person>
			<a href="/">
				<img src="img/purp.png" alt="" />

				<h1>This <br /> Person</h1></a
			>
		</person>

		<person>
			<a href="/">
				<img src="img/purp.png" alt="" />

				<h1>This <br /> Person</h1></a
			>
		</person>
	</staff>
</body>

<style lang="scss">
	@import 'components';

	staff {
		display: grid;
		grid-template-columns: 1fr 1fr 1fr;
		margin-bottom: 10%;
		margin-right: 8%;

		person {
			@include glassBack;
			margin: 3%;
			background: $backgroundThird;

			img {
				width: 100%;
			}

			h1 {
				margin-right: 10%;
			}

			h1 {
				margin: 0 30%;
			}
		}
	}
</style>
