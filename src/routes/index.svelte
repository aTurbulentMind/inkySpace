<body>
	<div class="art-banner" id="art-banner">
		<div class="art-banner-bg" />
		<div class="banner-text">Welcome</div>

		<div class="coaButt2">
			<p>
				<a href="https://www.facebook.com/OATHBremerton/"
					><svg
						xmlns="http://www.w3.org/2000/svg"
						xmlns:xlink="http://www.w3.org/1999/xlink"
						viewBox="0 0 24 24"
						><path
							d="M15.725 22v-7.745h2.6l.389-3.018h-2.99V9.31c0-.874.243-1.47 1.497-1.47h1.598v-2.7a21.391 21.391 0 0 0-2.33-.12c-2.304 0-3.881 1.407-3.881 3.99v2.227H10v3.018h2.607V22H3.104C2.494 22 2 21.506 2 20.896V3.104C2 2.494 2.494 2 3.104 2h17.792C21.506 2 22 2.494 22 3.104v17.792c0 .61-.494 1.104-1.104 1.104h-5.171z"
							fill="currentColor"
							fill-rule="evenodd"
						/></svg
					></a
				>
			</p>
			<p>
				<a href="https://www.instagram.com/OATHBremerton/"
					><svg
						xmlns="http://www.w3.org/2000/svg"
						xmlns:xlink="http://www.w3.org/1999/xlink"
						viewBox="0 0 256 256"
						><path
							d="M128 80a48 48 0 1 0 48 48a48 48 0 0 0-48-48zm0 80a32 32 0 1 1 32-32a32.1 32.1 0 0 1-32 32zm44-132H84a56 56 0 0 0-56 56v88a56 56 0 0 0 56 56h88a56 56 0 0 0 56-56V84a56 56 0 0 0-56-56zm40 144a40 40 0 0 1-40 40H84a40 40 0 0 1-40-40V84a40 40 0 0 1 40-40h88a40 40 0 0 1 40 40zm-20-96a12 12 0 1 1-12-12a12 12 0 0 1 12 12z"
							fill="currentColor"
						/></svg
					></a
				>
			</p>
		</div>
	</div>

	<h1>Things</h1>
	<p>
		Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus doloribus corporis quisquam
		perspiciatis? Expedita dolore unde ullam quisquam, repellat consectetur? Veniam in debitis hic
		quisquam!
	</p>

	<div class="icom">
		<a href="/staff">
			<h2>Meet Our People</h2>
			<img src="img/purp.png" alt="" /></a
		>
		<p>
			Lorem ipsum dolor sit amet consectetur adipisicing elit. Sit, sapiente voluptate. Nobis quae
			aliquid vitae rerum necessitatibus.
		</p>
	</div>

	<div class="icom">
		<a href="/story">
			<h2>Learn Our Story</h2>
			<img src="img/purp.png" alt="" /></a
		>
		<p>
			Lorem ipsum dolor sit, amet consectetur adipisicing elit. Amet atque accusantium at dolorum
			ipsum incidunt.
		</p>
	</div>

	<h1>Nice Words</h1>
	<h2>This Person</h2>
	<p>
		"Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus doloribus corporis quisquam
		perspiciatis? Expedita dolore unde ullam quisquam, repellat consectetur? Veniam in debitis hic
		quisquam!" &nbsp; &nbsp; &nbsp;
	</p>

	<h2>That Lady</h2>
	<p style="margin-bottom: 30%;">
		"Lorem ipsum, dolor sit amet consectetur adipisicing elit. Soluta alias quaerat doloremque! Qui
		debitis ad similique quibusdam recusandae consequuntur quaerat vitae illo!" &nbsp; &nbsp; &nbsp;
	</p>
</body>

<style lang="scss">
	@import 'components';

	h1,
	h2 {
		font-weight: 400;
	}

	.art-banner {
		height: 100vh;
		display: grid;
		background: $backgroundMain;
		grid-template-columns: 20px 1fr 1fr 1fr 20px;
		grid-template-rows: 20px 1fr 1fr 1fr 20px;
		margin: 5px 0;
		z-index: 99;

		a {
			font-size: 3vw;
		}

		&::before {
			content: '';
			opacity: 0.85;
			border-top: 5px solid $backgroundSecond;
			border-right: 5px solid $backgroundSecond;
			grid-column: 4;
			grid-row: 1 / span 4;
			z-index: 2;
		}

		&::after {
			content: '';
			opacity: 0.85;
			border-bottom: 5px solid $backgroundSecond;
			border-left: 5px solid $backgroundSecond;
			grid-column: 2;
			grid-row: span 4 / 5;
			z-index: 2;
		}
	}

	.art-banner-bg {
		background-image: url(/img/blackLogo.jpg);
		background-repeat: no-repeat;
		background-attachment: fixed;
		background-position: top;
		background-size: 90%;
		opacity: 0.15;
		grid-column: 1 / -1;
		grid-row: 1 / -1;

		img {
			width: 100%;
			padding: 15%;
		}
	}

	.banner-text {
		font-size: 10vw;
		font-weight: bold;
		grid-column: 2 / span 2;
		grid-row: 3 /* no need to type one*/;
		align-self: center;
		justify-self: center;
	}

	.coaButt2 {
		display: grid;
		align-self: center;
		justify-self: center;
		grid-column: 3 / 5;
		grid-row: 4 / 4;
		background-color: $backgroundSecond;
		font-weight: bold;
		width: 10vw;
		height: 15vw;
		border-radius: 50%;
		transform: rotate(4deg);

		p {
			margin: auto;
			font-family: $altFont;
		}

		SVG {
			width: 30%;
			height: 30%;
			margin: 0 35%;
			color: $textColorMain;
		}
	}

	.icom {
		img {
			max-width: 100%;
		}
	}

	@media (min-width: 750px) {
		.art-banner-bg {
			background-size: 70%;
		}

		p {
			margin-left: 15%;
		}
	}

	@media (min-width: 1000px) {
		.art-banner-bg {
			background-size: 50%;
		}
	}
</style>
