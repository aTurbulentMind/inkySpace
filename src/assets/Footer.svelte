<div class="footer">
	<h1>ORCA HOUSE TATTOO HOUSE</h1>
	<footBox>
		<ul>
			<li><a href="/">HOME</a></li>
			<li><a href="/">CONTACT</a></li>
			<li><a href="/">(360)555-5555</a></li>
			<li><a href="/">GALLERY</a></li>
			<li><a href="/">OUR STORY</a></li>
		</ul>
	</footBox>
	<footBox>
		<ul>
			<li><a href="/">STAFF:</a></li>
			<li><a href="/">BONNIE</a></li>
			<li><a href="/">JESSIE</a></li>
		</ul>
	</footBox>
	<footBox />
	<footBox />
	<footBox>
		<socBox>
			<a href="/"
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

			<a href="/"
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

			<a href="/"
				><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"
					><path
						fill="currentColor"
						d="M23.643 4.937c-.835.37-1.732.62-2.675.733a4.67 4.67 0 0 0 2.048-2.578a9.3 9.3 0 0 1-2.958 1.13a4.66 4.66 0 0 0-7.938 4.25a13.229 13.229 0 0 1-9.602-4.868c-.4.69-.63 1.49-.63 2.342A4.66 4.66 0 0 0 3.96 9.824a4.647 4.647 0 0 1-2.11-.583v.06a4.66 4.66 0 0 0 3.737 4.568a4.692 4.692 0 0 1-2.104.08a4.661 4.661 0 0 0 4.352 3.234a9.348 9.348 0 0 1-5.786 1.995a9.5 9.5 0 0 1-1.112-.065a13.175 13.175 0 0 0 7.14 2.093c8.57 0 13.255-7.098 13.255-13.254c0-.2-.005-.402-.014-.602a9.47 9.47 0 0 0 2.323-2.41l.002-.003Z"
					/></svg
				></a
			>
		</socBox>
	</footBox>
</div>

<style lang="scss">
	@import '../src/routes/components';

	.footer {
		display: grid;
		background: $gradient;

		grid-template-columns: 1fr 1fr 1fr;

		footBox {
			margin: 8% 0 0 0;
			h1 {
				margin: 5%;
			}

			ul {
				position: relative;
				margin: 10% 5% -8% 5%;
				list-style: none;

				li {
					margin: 1%;
					padding: 1%;

					a {
						color: $textColorMain;
						text-decoration: underline;
					}
				}
			}
			socBox {
				margin: 2% 0 0 -10%;
				SVG {
					background: $textColorMain;
					color: $backgroundMain;
					border-radius: 50%;
					margin: 3%;
					padding: 3%;
					width: 10%;
				}
			}
		}
	}
</style>
