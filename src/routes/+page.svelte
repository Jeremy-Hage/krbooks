<div id="app-container">
	<nav>i am the nav bar</nav>
	<main>
		<div id="header">
			<div>
				<h1>Welcome to ...</h1>

				<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
			</div>
		</div>
		<div id="search">
			<div>
				<a href="/">what color?</a>
			</div>
			<div>
				<input placeholder="Search for something" />
				<button>why not pretty?</button>
			</div>
		</div>
		<footer>some footer</footer>
	</main>
</div>

<style>
	#app-container {
		display: grid;
		grid-auto-rows: 50px 1fr;
		min-height: 100vh;
	}
	nav {
		background-color: var(--surface-2);
	}
	main {
		display: grid;
		grid-template-rows: 1fr 3fr 50px;
	}
	#header {
		display: grid;
		grid-template-columns: 1fr 3fr 1fr;
	}
	#header > div {
		display: flex;
		flex-direction: column;
		padding-inline: 1rem;
		grid-column: 2/ 3;
	}
	#search {
		display: grid;
		grid-template-columns: 1fr 3fr 1fr;
	}
	#search > div {
		display: flex;
		flex-direction: column;
		padding-inline: 1rem;
		grid-column: 2/ 3;
	}
</style>
