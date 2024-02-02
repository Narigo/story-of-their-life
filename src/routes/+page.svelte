<script lang="ts">
	const deckOne: string[] = [];
	const deckTwo: string[] = [];
</script>

<div class="body">
	<section class="board">
		<button on:click={() => {}} class="deck job"></button>
		<button on:click={() => {}} class="deck termination"></button>
		<div class="card job"></div>
		<div class="card termination"></div>
	</section>
</div>

<style>
	.body {
		display: grid;
		place-items: center;
	}

	.deck,
	.card {
		border: 2px solid black;
		border-radius: 12px;
		height: 300px;
		width: 200px;
		position: absolute;
	}

	.card {
		border: 2px dashed black;
	}

	.deck {
		top: 0;
	}

	.card {
		bottom: 0;
	}

	.job {
		left: 0;
	}
	.termination {
		right: 0;
	}

	.deck.job {
		background: blue;
	}
	.deck.termination {
		background: green;
	}

	.board {
		position: relative;
		border: 1px solid red;
		height: 700px;
		width: 500px;
	}
</style>
