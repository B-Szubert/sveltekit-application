<script>
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Home" />
</svelte:head>

<section>
	<h1>
		To jest stona z przepisami
	</h1>

	<h2>
		Strona z przepisami kulinarnymi jest miejscem, gdzie użytkownicy mogą znaleźć i udostępniać różnorodne przepisy na potrawy. Ta konkretna strona zawiera sekcję zatytułowaną "To jest stona z przepisami", która wyświetla nagłówek o tej samej treści. Jest to główny element strony, który przyciąga uwagę użytkowników i informuje ich o tematyce strony. Ponadto, strona zawiera również pusty nagłówek drugiego poziomu, który może być wykorzystany do wyświetlania dodatkowych informacji lub tytułów sekcji.
	</h2>

</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	h1 {
		width: 100%;
	}

	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
</style>
