<svelte:head>
	<title>Add</title>
	<meta name="description" content="Add new recepy" />
</svelte:head>

<div class="text-column">
	<h1>Dodaj przepis</h1>
	
	<form>
		<div class="form-group">
			<label for="nazwa">nazwa</label>
			<input type="text" id="nazwa" name="nazwa" />
		</div>
		
		<div class="form-group">
			<label for="skladniki">skladniki</label>
			<textarea id="skladniki" name="skladniki"></textarea>
		</div>
		
		<div class="form-group">
			<label for="instrukcje">instrukcje</label>
			<textarea id="instrukcje" name="instrukcje"></textarea>
		</div>
		
		<button class="submit-button" type="submit">dodaj przepis</button>
	</form>
</div>

<style>
    .text-column {
        width: 100%;
        max-width: 600px;
        margin: 0 auto;
    }

    .form-group {
        margin-bottom: 1rem;
    }

    label {
        display: block;
        margin-bottom: 0.5rem;
    }

    input, textarea {
        width: 100%;
        padding: 0.5rem;
        border: 1px solid #ccc;
        border-radius: 4px;
    }

    .submit-button {
        padding: 0.5rem 1rem;
        background-color: #007BFF;
        color: white;
		font-size: medium;
        border: none;
		min-width: 100px;
        border-radius: 4px;
        cursor: pointer;
    }

    .submit-button:hover {
        background-color: #0056b3;
    }
</style>
