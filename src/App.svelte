<script>
	import Footer from './components/Footer.svelte'
	export let name;
</script>

<svelte:head>
	<meta name="viewport" content="width=device-width, initial-scale=1">
</svelte:head>

<main>
	<h1>Hello {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</main>
<Footer />

<style>
	:global(html) {
		font-size: 62.5%;
	}

	@media (max-width: 768px) {
		:global(html) {
			font-size: 50%;
		}
	}
	@media screen and (min-width: 768px) and (max-width: 1023px) {
    	:global(html) {
			font-size: 100%;
		}
    }
    @media screen and (min-width: 1024px) {
    	:global(html) {
			font-size: 200%;
		}
    }

	main {
		text-align: center;
		padding: 2rem;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

</style>